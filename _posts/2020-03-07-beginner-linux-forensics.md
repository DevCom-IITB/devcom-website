---
layout: post
title:  "We think we're owned..."
tagline: Beginner Linux Forensics
date: 2020-03-07 16:32
categories: [Tasks]
tags: [Easy, tasks, tools]
image: ubuntu-linux.jpg
---

## Thanks
<p>&nbsp;</p>
I'd like to say a big thanks to my friend Angry Bender for their explanation of Linux kernels. I would be lost without it. 

If you'd like to check out their stuff head over to [angry-bender](https://angry-bender.github.io)
<p>&nbsp;</p>
## Foreword
<p>&nbsp;</p>
If you need some help setting up a profile jump past the scenario to the setup section.

I'd also like to note that before this point my linux forensics experience was very limited. The task itself I found easy however what I got the most out of before and even after was the learning about Linux kernels.
<p>&nbsp;</p>
## Scenario
<p>&nbsp;</p>
Your SOC has left a USB with a sticky note on it.

> We have received a report of an IP owned by your company 192.168.32.128 has been communicating with malicious IP 192.168.32.129.
<p>&nbsp;</p>
[uctf.zip](https://drive.google.com/uc?export=view&id=1BIVNenWrT57dJ39kgFTngVZMjyk5Q7KI)
<p>&nbsp;</p>
## Task
<p>&nbsp;</p>
Your manager wants the following answered ASAP.

(1.) Can you download the file and produce the md5 of the vmem file?

(2.) What is the CVE used for the initial access onto the system? (Format CVE-year-number)

(3.) What is the md5 of the ELF implant in memory? (Note this is the only question you really need volatility for).

(4.) What is the _tool_ used to create and implement the ELF binary? 

(5.) What is the full path, including the filename, of the webshell?

(6.) What is the command executed via the webshell?
<p>&nbsp;</p>
## Planning
<p>&nbsp;</p>
You've already set up your volatility profile and you have everything you need. For your planning think about where this information would be on a system and start looking in those places first.
<p>&nbsp;</p>
## Tools
<p>&nbsp;</p>
Two tools will get you nearly everything `volatility` and `strings`.
<p>&nbsp;</p>
## Setup
<p>&nbsp;</p>
The initial resources given were: System.map-2.6.24-16-server, uctf.vmem.

The vmem file is a virual memory file that can be obtained when you suspend a virtual machine and copy it out of the directory it is being held in. 

The System map file will help us create the profile to use with volatility. 

The first step is to determine what kind of Linux system we're working with since the system admin that we got it from has gone to Hawaii for two weeks while the place burns down around us. 

Linux memory files are rich with information since it is mostly text based so let's `grep` for Linux.
<p>&nbsp;</p>
![Search for Linux](https://cybercodebear.github.io/images/blog/easy-linux-forensics/searchforlinux.png)
<p>&nbsp;</p>
This gives a lot of results but if we check near the top we can see that we're looking at an Unbuntu system and the numbers match the System map file. 

Next we need the codename associated with this kernel so that we can download the correct profile from github.

Now I don't know much about Ubuntu since I mostly just use Kali so let's see what Ubuntu is based on.
<p>&nbsp;</p>
![What is Ubuntu based on?](https://cybercodebear.github.io/images/blog/easy-linux-forensics/ubuntubase.png)
<p>&nbsp;</p>
Great! But now I don't know how to find the codename in the memory image. After some searching I found this [blog](https://phoenixnap.com/kb/how-to-update-kernel-ubuntu) that explains how to update a kernel on a debian based system. 
<p>&nbsp;</p>
![Kernel updates](https://cybercodebear.github.io/images/blog/easy-linux-forensics/kernelupdate.png)
<p>&nbsp;</p>
The above image shows the kernel updating and what we may find in memory, so let's do a search for a partial URL. Using the following command `strings uctf.vmem |grep '\/ubuntu\/'`
<p>&nbsp;</p>
![Codename search](https://cybercodebear.github.io/images/blog/easy-linux-forensics/codenamesearch.png)
<p>&nbsp;</p>
Hmm hardy looks good, maybe another google search.
<p>&nbsp;</p>
![Hardy Ubuntu](https://cybercodebear.github.io/images/blog/easy-linux-forensics/hardyubuntu.png)
<p>&nbsp;</p>
Now the above search isn't foolproof so let me show you what else you could search for. 
<p>&nbsp;</p>
![Other codenames](https://cybercodebear.github.io/images/blog/easy-linux-forensics/othercodenames.png)
<p>&nbsp;</p>
These two searches did give something but there are also some other searches you could try that aren't in this particular memory image; `VERSION=` and `PRETTY_NAME=`.

Note this may change between Linux releases so it's important to do your research and see how each type will update that kernel which can lead you down the correct path. 

Looks like we've found our match. Now let's check the [release history](https://wiki.ubuntu.com/Releases).

The line we're interested is found by searching for `hardy` and gives us; Ubuntu 8.04.4 LTS.

The numbers are what we need to select a profile from the Volatility Foundation [profiles page](https://github.com/volatilityfoundation/profiles/tree/master/Linux/Ubuntu/x86).

Go ahead and download the `Ubuntu8044.zip` and store it in our working directory. 

Now we need some background on how profile are normally created, go and read this [page](https://github.com/volatilityfoundation/volatility/wiki/Linux).

It boils down to the fact you need to zip up a System map and module.dwarf file and store it somewhere. However, we already have a System map file that was given as a resource so let's use that.

Below is a speed run of the commands needed to do this task. 
<p>&nbsp;</p>
![Command speed run](https://cybercodebear.github.io/images/blog/easy-linux-forensics/speedrun.png)
<p>&nbsp;</p>
Let's check if the profile has been added.
<p>&nbsp;</p>
![Profile check](https://cybercodebear.github.io/images/blog/easy-linux-forensics/profilecheck.png)
<p>&nbsp;</p>
Great! Now finally the basic test we do with profiles is to test a `pslist` or in this case a `linux_pslist`.
<p>&nbsp;</p>
![Vol check](https://cybercodebear.github.io/images/blog/easy-linux-forensics/linux_pslist.png)
<p>&nbsp;</p>
Now that we're all set up let's get into the scenario back up the top.
<p>&nbsp;</p>
## Solution
<p>&nbsp;</p>
[![](https://img.youtube.com/vi/aE3lBIn3MlQ/maxresdefault.jpg)](https://youtu.be/aE3lBIn3MlQ)

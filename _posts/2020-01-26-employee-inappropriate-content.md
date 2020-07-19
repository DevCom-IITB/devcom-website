---
layout: post
title:  "Inappropriate Content"
tagline: Prove an employee accessed
date: 2020-01-26 10:04
categories: [Tasks]
tags: [Very Easy, tasks, tools, forensics]
image: noporn.jpg
---

## Scenario
<p>&nbsp;</p> 
The company you work for supplies employees with a laptop to take away for work so that they can VPN back into the company servers. Everytime an employee loans a laptop from the IT they must sign an appropriate use form which states the laptop can only be used for work purposes. 

An employee who recently has loaned out a laptop has noticed in the recent documents section within Explorer there are video files that look like adult content. Since this would constitute inappropriate behaviour the employee reported this to management and they have come to you as the analyst to figure out who it was. Below is an image of what the reporting employee saw.
<p>&nbsp;</p>
![Image of content seen](https://cybercodebear.github.io/images/blog/inaprop_content/content_proof.jpg)

The system admin has also collected some data for you before reimaging the laptop. Hopefully this is enough for your investigation.... oh and the system admin also told you that everyone uses the same IEUser account and they just track who the laptop is loaned out to in a text file.
<p>&nbsp;</p> 
## Task 
<p>&nbsp;</p>
For a small task like this you will most likely have a good idea of what you'll need to find but it is good practice to put pen to paper and write out a small plan of the evidence that you will need and roughly what tools you will use.
<p>&nbsp;</p>
## Attempt the task
<p>&nbsp;</p>
Below the task files section is the solution along with my own thought process for this task. If you have some ability then plan out the task, download the content on this page, and attempt to complete this before looking at what I have done. 
<p>&nbsp;</p>
## Task files
<p>&nbsp;</p>
Download the files by clicking on the icon below;
<p>&nbsp;</p>
[![button](https://cybercodebear.github.io/images/blog/inaprop_content/vm-icon-png-icon.jpg)](https://cybercodebear.github.io/images/blog/downloads/Prove-an-employee-viewed-inappropriate-content.7z)
<p>&nbsp;</p>
## Solution: Video
<p>&nbsp;</p>
I have now created a video that will step through how to, create the VM's to make this task; acquire the data that was downloaded in the zip; do the task.
<p>&nbsp;</p>
[![Alt text](http://i3.ytimg.com/vi/0oLy34oPzw0/maxresdefault.jpg)](https://youtu.be/0oLy34oPzw0)
<p>&nbsp;</p>
### Planning
<p>&nbsp;</p>
When I initially got this task the first thing I did was fire up the laptop and had a look at what the employee who reported the issue could see. This was to confirm that they were telling the truth and that it would be worth while continuing further. I was not worried about overriding evidence because I didn't plan on opening any files that would overwrite this list.
<p>&nbsp;</p>
![Image of content seen](https://cybercodebear.github.io/images/blog/inaprop_content/content_proof.jpg)

As we can see from above it looks like a user has been looking at inappropriate content with those names. To bad the output doesn't give us the date and time it was plugged in.

### Tools
<p>&nbsp;</p>
What we do have is that these files are listed under the *Recent Files* heading in explorer. I know from experience I'm probably going to want to look in the registry (using [Registry Explorer](https://ericzimmerman.github.io/#!index.md)) for the values associated with this key to hopefully get an answer. 

Registry Explorer is ideal because it collates a lot of information I would normally have to do myself. I will add a section on Zimmerman tools that I use in the [analyst playbook](https://cybercodebear.github.io/analyst-playbook) later.

### Research
<p>&nbsp;</p>
Let's google where we might be able to find the key we're after. The google search I used was;
<p>&nbsp;</p>
![google search](https://cybercodebear.github.io/images/blog/inaprop_content/google-search.png)

Looking down the page I can see that a NirSoft blog that may be interesting;
<p>&nbsp;</p>
![4th result](https://cybercodebear.github.io/images/blog/inaprop_content/4th-result.png)

Now remember that the user that we currently have data for is the IEUser. With that in mind load up the *NTUSER.dat* hive.

### First look
<p>&nbsp;</p>
Run Registry Explorer on your Windows machine and then go *File > Open Hive* like in the picture below. 
<p>&nbsp;</p>
![Open hive](https://cybercodebear.github.io/images/blog/inaprop_content/load-hive.png)

Then for the next image select *No*.
<p>&nbsp;</p>
![Combine hive](https://cybercodebear.github.io/images/blog/inaprop_content/combine-hive.png)

The when it asks you to load a dirty hive, select *Yes*.
<p>&nbsp;</p>
![Dirty hive](https://cybercodebear.github.io/images/blog/inaprop_content/dirty-hive.png)

Hmm the key that NirSoft told us to go to, *HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\ComDlg32\OpenSaveMRU*, has somethings that appear in that recent file list but not the ones we're after.

### More research
<p>&nbsp;</p>
Let's turn back to the google search and look further. Maybe two search results down might help. 
<p>&nbsp;</p>
![further reseach](https://cybercodebear.github.io/images/blog/inaprop_content/further-research.png)

After reading the [blog](https://www.nextofwindows.com/windows-10-tip-how-to-clean-up-file-explorer-recent-history) the *typedpaths* key looks like it might be good to try. 

### Second look
<p>&nbsp;</p>
Navigating to it in Regsitry Explorer gives the following;
<p>&nbsp;</p>
![typedpaths](https://cybercodebear.github.io/images/blog/inaprop_content/my-typed-paths.png)

### Analyst's hunch
<p>&nbsp;</p>
Buh-bow doesn't look good for us. However that's two keys in the same parent key! So maybe I might just click around in, *HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer*, and see what I can find in here....
<p>&nbsp;</p>
![my recentdocs](https://cybercodebear.github.io/images/blog/inaprop_content/my-recentdocs.png)

Would you look at that! The subkey breaks down into file types. I know from the original evidence I'm looking for mp4 files and now I have the files I'm after and a time stamp, 2019-12-21 09:12:29!

### Connecting the dots
<p>&nbsp;</p>
Now all I need to do is compare the loaned laptop list with the time stamp and I'll have the answer. 
<p>&nbsp;</p>
![loan history](https://cybercodebear.github.io/images/blog/inaprop_content/loan-history.png)

Well it looks like the culprit is Navid Flyde, make sure you do a report and submit this to your manager before archiving the evidence. 

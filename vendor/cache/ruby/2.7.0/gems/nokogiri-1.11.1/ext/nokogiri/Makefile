
SHELL = /bin/sh

# V=0 quiet, V=1 verbose.  other values don't work.
V = 0
Q1 = $(V:1=)
Q = $(Q1:0=@)
ECHO1 = $(V:1=@ :)
ECHO = $(ECHO1:0=@ echo)
NULLCMD = :

#### Start of system configuration section. ####

srcdir = .
topdir = /usr/include/ruby-2.7.0
hdrdir = $(topdir)
arch_hdrdir = /usr/include/x86_64-linux-gnu/ruby-2.7.0
PATH_SEPARATOR = :
VPATH = $(srcdir):$(arch_hdrdir)/ruby:$(hdrdir)/ruby
prefix = $(DESTDIR)/usr
rubysitearchprefix = $(sitearchlibdir)/$(RUBY_BASE_NAME)
rubyarchprefix = $(archlibdir)/$(RUBY_BASE_NAME)
rubylibprefix = $(libdir)/$(RUBY_BASE_NAME)
exec_prefix = $(prefix)
vendorarchhdrdir = $(sitearchincludedir)/$(RUBY_VERSION_NAME)/vendor_ruby
sitearchhdrdir = $(sitearchincludedir)/$(RUBY_VERSION_NAME)/site_ruby
rubyarchhdrdir = $(archincludedir)/$(RUBY_VERSION_NAME)
vendorhdrdir = $(rubyhdrdir)/vendor_ruby
sitehdrdir = $(rubyhdrdir)/site_ruby
rubyhdrdir = $(includedir)/$(RUBY_VERSION_NAME)
vendorarchdir = $(rubysitearchprefix)/vendor_ruby/$(ruby_version)
vendorlibdir = $(vendordir)/$(ruby_version)
vendordir = $(rubylibprefix)/vendor_ruby
sitearchdir = $(DESTDIR)./.gem.20210527-19367-1550h3f
sitelibdir = $(DESTDIR)./.gem.20210527-19367-1550h3f
sitedir = $(DESTDIR)/usr/local/lib/site_ruby
rubyarchdir = $(rubyarchprefix)/$(ruby_version)
rubylibdir = $(rubylibprefix)/$(ruby_version)
sitearchincludedir = $(includedir)/$(sitearch)
archincludedir = $(includedir)/$(arch)
sitearchlibdir = $(libdir)/$(sitearch)
archlibdir = $(libdir)/$(arch)
ridir = $(datarootdir)/$(RI_BASE_NAME)
mandir = $(datarootdir)/man
localedir = $(datarootdir)/locale
libdir = $(exec_prefix)/lib
psdir = $(docdir)
pdfdir = $(docdir)
dvidir = $(docdir)
htmldir = $(docdir)
infodir = $(datarootdir)/info
docdir = $(datarootdir)/doc/$(PACKAGE)
oldincludedir = $(DESTDIR)/usr/include
includedir = $(prefix)/include
runstatedir = $(DESTDIR)/var/run
localstatedir = $(DESTDIR)/var
sharedstatedir = $(prefix)/com
sysconfdir = $(DESTDIR)/etc
datadir = $(datarootdir)
datarootdir = $(prefix)/share
libexecdir = $(exec_prefix)/libexec
sbindir = $(exec_prefix)/sbin
bindir = $(exec_prefix)/bin
archdir = $(rubyarchdir)


CC_WRAPPER = 
CC = gcc
CXX = g++
LIBRUBY = $(LIBRUBY_SO)
LIBRUBY_A = lib$(RUBY_SO_NAME)-static.a
LIBRUBYARG_SHARED = -l$(RUBY_SO_NAME)
LIBRUBYARG_STATIC = -l$(RUBY_SO_NAME)-static $(MAINLIBS)
empty =
OUTFLAG = -o $(empty)
COUTFLAG = -o $(empty)
CSRCFLAG = $(empty)

RUBY_EXTCONF_H = 
cflags   = $(optflags) $(debugflags) $(warnflags)
cxxflags = 
optflags = -O3
debugflags = -ggdb3
warnflags = -Wall -Wextra -Wdeprecated-declarations -Wduplicated-cond -Wimplicit-function-declaration -Wimplicit-int -Wmisleading-indentation -Wpointer-arith -Wwrite-strings -Wimplicit-fallthrough=0 -Wmissing-noreturn -Wno-cast-function-type -Wno-constant-logical-operand -Wno-long-long -Wno-missing-field-initializers -Wno-overlength-strings -Wno-packed-bitfield-compat -Wno-parentheses-equality -Wno-self-assign -Wno-tautological-compare -Wno-unused-parameter -Wno-unused-value -Wsuggest-attribute=format -Wsuggest-attribute=noreturn -Wunused-variable
cppflags = 
CCDLFLAGS = -fPIC
CFLAGS   = $(CCDLFLAGS) -g -O2 -fdebug-prefix-map=/build/ruby2.7-2E2p8v/ruby2.7-2.7.0=. -fstack-protector-strong -Wformat -Werror=format-security -fPIC -g -Winline -Wmissing-noreturn $(ARCH_FLAG)
INCFLAGS = -I. -I$(arch_hdrdir) -I$(hdrdir)/ruby/backward -I$(hdrdir) -I$(srcdir)
DEFS     = 
CPPFLAGS = -DHAVE_XMLPARSEDOC -DHAVE_XSLTPARSESTYLESHEETDOC -DHAVE_EXSLTFUNCREGISTER -DHAVE_XMLHASFEATURE -DHAVE_XMLFIRSTELEMENTCHILD -DHAVE_XMLRELAXNGSETPARSERSTRUCTUREDERRORS -DHAVE_XMLRELAXNGSETVALIDSTRUCTUREDERRORS -DHAVE_XMLSCHEMASETVALIDSTRUCTUREDERRORS -DHAVE_XMLSCHEMASETPARSERSTRUCTUREDERRORS -DHAVE_VASPRINTF -I/home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxml2/2.9.10/include/libxml2 -I/home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxslt/1.1.34/include -I/home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxml2/2.9.10/include/libxml2 -Wdate-time -D_FORTIFY_SOURCE=2 $(DEFS) $(cppflags) -DNOKOGIRI_PACKAGED_LIBRARIES -DNOKOGIRI_LIBXML2_PATCHES="\"0001-Revert-Do-not-URI-escape-in-server-side-includes.patch 0002-Remove-script-macro-support.patch 0003-Update-entities-to-remove-handling-of-ssi.patch 0004-libxml2.la-is-in-top_builddir.patch 0005-Fix-infinite-loop-in-xmlStringLenDecodeEntities.patch 0006-htmlParseComment-treat-as-if-it-closed-the-comment.patch 0007-use-new-htmlParseLookupCommentEnd-to-find-comment-en.patch 0008-use-glibc-strlen.patch 0009-avoid-isnan-isinf.patch\"" -DNOKOGIRI_LIBXSLT_PATCHES="\"\"" -DNOKOGIRI_OTHER_LIBRARY_VERSIONS="\"\""
CXXFLAGS = $(CCDLFLAGS) -g -O2 -fdebug-prefix-map=/build/ruby2.7-2E2p8v/ruby2.7-2.7.0=. -fstack-protector-strong -Wformat -Werror=format-security $(ARCH_FLAG)
ldflags  = -L. -Wl,-Bsymbolic-functions -Wl,-z,relro -Wl,-z,now -fstack-protector-strong -rdynamic -Wl,-export-dynamic
dldflags = -Wl,-Bsymbolic-functions -Wl,-z,relro -Wl,-z,now 
ARCH_FLAG = 
DLDFLAGS = $(ldflags) $(dldflags) $(ARCH_FLAG)
LDSHARED = $(CC) -shared
LDSHAREDXX = $(CXX) -shared
AR = ar
EXEEXT = 

RUBY_INSTALL_NAME = $(RUBY_BASE_NAME)2.7
RUBY_SO_NAME = ruby-2.7
RUBYW_INSTALL_NAME = 
RUBY_VERSION_NAME = $(RUBY_BASE_NAME)-$(ruby_version)
RUBYW_BASE_NAME = rubyw
RUBY_BASE_NAME = ruby

arch = x86_64-linux-gnu
sitearch = $(arch)
ruby_version = 2.7.0
ruby = $(bindir)/$(RUBY_BASE_NAME)2.7
RUBY = $(ruby)
ruby_headers = $(hdrdir)/ruby.h $(hdrdir)/ruby/backward.h $(hdrdir)/ruby/ruby.h $(hdrdir)/ruby/defines.h $(hdrdir)/ruby/missing.h $(hdrdir)/ruby/intern.h $(hdrdir)/ruby/st.h $(hdrdir)/ruby/subst.h $(arch_hdrdir)/ruby/config.h

RM = rm -f
RM_RF = $(RUBY) -run -e rm -- -rf
RMDIRS = rmdir --ignore-fail-on-non-empty -p
MAKEDIRS = /bin/mkdir -p
INSTALL = /usr/bin/install -c
INSTALL_PROG = $(INSTALL) -m 0755
INSTALL_DATA = $(INSTALL) -m 644
COPY = cp
TOUCH = exit >

#### End of system configuration section. ####

preload = 
libpath = . $(archlibdir) /home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxml2/2.9.10/lib /home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxslt/1.1.34/lib
LIBPATH =  -L. -L$(archlibdir) -L/home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxml2/2.9.10/lib -L/home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxslt/1.1.34/lib
DEFFILE = 

CLEANFILES = mkmf.log
DISTCLEANFILES = 
DISTCLEANDIRS = 

extout = 
extout_prefix = 
target_prefix = /nokogiri
LOCAL_LIBS = 
LIBS = $(LIBRUBYARG_SHARED) /home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxslt/1.1.34/lib/libexslt.a -lm -ldl -lz /home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxml2/2.9.10/lib/libxml2.a /home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxslt/1.1.34/lib/libxslt.a -ldl -lm -lz /home/dev/Desktop/devcom/devcomiitb.github.io/vendor/cache/ruby/2.7.0/gems/nokogiri-1.11.1/ports/x86_64-pc-linux-gnu/libxml2/2.9.10/lib/libxml2.a -lm   -lc
ORIG_SRCS = html_document.c html_element_description.c html_entity_lookup.c html_sax_parser_context.c html_sax_push_parser.c nokogiri.c test_global_handlers.c xml_attr.c xml_attribute_decl.c xml_cdata.c xml_comment.c xml_document.c xml_document_fragment.c xml_dtd.c xml_element_content.c xml_element_decl.c xml_encoding_handler.c xml_entity_decl.c xml_entity_reference.c xml_io.c xml_libxml2_hacks.c xml_namespace.c xml_node.c xml_node_set.c xml_processing_instruction.c xml_reader.c xml_relax_ng.c xml_sax_parser.c xml_sax_parser_context.c xml_sax_push_parser.c xml_schema.c xml_syntax_error.c xml_text.c xml_xpath_context.c xslt_stylesheet.c
SRCS = $(ORIG_SRCS) 
OBJS = html_document.o html_element_description.o html_entity_lookup.o html_sax_parser_context.o html_sax_push_parser.o nokogiri.o test_global_handlers.o xml_attr.o xml_attribute_decl.o xml_cdata.o xml_comment.o xml_document.o xml_document_fragment.o xml_dtd.o xml_element_content.o xml_element_decl.o xml_encoding_handler.o xml_entity_decl.o xml_entity_reference.o xml_io.o xml_libxml2_hacks.o xml_namespace.o xml_node.o xml_node_set.o xml_processing_instruction.o xml_reader.o xml_relax_ng.o xml_sax_parser.o xml_sax_parser_context.o xml_sax_push_parser.o xml_schema.o xml_syntax_error.o xml_text.o xml_xpath_context.o xslt_stylesheet.o
HDRS = $(srcdir)/xml_libxml2_hacks.h $(srcdir)/xml_namespace.h $(srcdir)/xml_attr.h $(srcdir)/xml_text.h $(srcdir)/xslt_stylesheet.h $(srcdir)/xml_sax_push_parser.h $(srcdir)/xml_relax_ng.h $(srcdir)/xml_cdata.h $(srcdir)/xml_sax_parser_context.h $(srcdir)/html_element_description.h $(srcdir)/xml_entity_reference.h $(srcdir)/xml_dtd.h $(srcdir)/xml_attribute_decl.h $(srcdir)/html_sax_parser_context.h $(srcdir)/xml_io.h $(srcdir)/html_sax_push_parser.h $(srcdir)/xml_element_content.h $(srcdir)/xml_reader.h $(srcdir)/xml_node_set.h $(srcdir)/xml_element_decl.h $(srcdir)/xml_sax_parser.h $(srcdir)/html_entity_lookup.h $(srcdir)/html_document.h $(srcdir)/xml_document_fragment.h $(srcdir)/xml_xpath_context.h $(srcdir)/xml_node.h $(srcdir)/xml_processing_instruction.h $(srcdir)/xml_entity_decl.h $(srcdir)/xml_document.h $(srcdir)/xml_comment.h $(srcdir)/nokogiri.h $(srcdir)/xml_schema.h $(srcdir)/xml_syntax_error.h $(srcdir)/xml_encoding_handler.h
LOCAL_HDRS = 
TARGET = nokogiri
TARGET_NAME = nokogiri
TARGET_ENTRY = Init_$(TARGET_NAME)
DLLIB = $(TARGET).so
EXTSTATIC = 
STATIC_LIB = 

TIMESTAMP_DIR = .
BINDIR        = $(bindir)
RUBYCOMMONDIR = $(sitedir)$(target_prefix)
RUBYLIBDIR    = $(sitelibdir)$(target_prefix)
RUBYARCHDIR   = $(sitearchdir)$(target_prefix)
HDRDIR        = $(rubyhdrdir)/ruby$(target_prefix)
ARCHHDRDIR    = $(rubyhdrdir)/$(arch)/ruby$(target_prefix)
TARGET_SO_DIR =
TARGET_SO     = $(TARGET_SO_DIR)$(DLLIB)
CLEANLIBS     = $(TARGET_SO) 
CLEANOBJS     = *.o  *.bak

all:    $(DLLIB)
static: $(STATIC_LIB)
.PHONY: all install static install-so install-rb
.PHONY: clean clean-so clean-static clean-rb

clean-static::
clean-rb-default::
clean-rb::
clean-so::
clean: clean-so clean-static clean-rb-default clean-rb
		-$(Q)$(RM) $(CLEANLIBS) $(CLEANOBJS) $(CLEANFILES) .*.time

distclean-rb-default::
distclean-rb::
distclean-so::
distclean-static::
distclean: clean distclean-so distclean-static distclean-rb-default distclean-rb
		-$(Q)$(RM) Makefile $(RUBY_EXTCONF_H) conftest.* mkmf.log
		-$(Q)$(RM) core ruby$(EXEEXT) *~ $(DISTCLEANFILES)
		-$(Q)$(RMDIRS) $(DISTCLEANDIRS) 2> /dev/null || true

realclean: distclean
install: install-so install-rb

install-so: $(DLLIB) $(TIMESTAMP_DIR)/.sitearchdir.-.nokogiri.time
	$(INSTALL_PROG) $(DLLIB) $(RUBYARCHDIR)
clean-static::
	-$(Q)$(RM) $(STATIC_LIB)
install-rb: pre-install-rb do-install-rb install-rb-default
install-rb-default: pre-install-rb-default do-install-rb-default
pre-install-rb: Makefile
pre-install-rb-default: Makefile
do-install-rb:
do-install-rb-default:
pre-install-rb-default:
	@$(NULLCMD)
pre-install-rb: $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/DOCBparser.h
$(RUBYLIBDIR)/include/libxml2/libxml/DOCBparser.h: $(srcdir)/include/libxml2/libxml/DOCBparser.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/DOCBparser.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlsave.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlsave.h: $(srcdir)/include/libxml2/libxml/xmlsave.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlsave.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlautomata.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlautomata.h: $(srcdir)/include/libxml2/libxml/xmlautomata.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlautomata.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlstring.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlstring.h: $(srcdir)/include/libxml2/libxml/xmlstring.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlstring.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/uri.h
$(RUBYLIBDIR)/include/libxml2/libxml/uri.h: $(srcdir)/include/libxml2/libxml/uri.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/uri.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/HTMLtree.h
$(RUBYLIBDIR)/include/libxml2/libxml/HTMLtree.h: $(srcdir)/include/libxml2/libxml/HTMLtree.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/HTMLtree.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/schemasInternals.h
$(RUBYLIBDIR)/include/libxml2/libxml/schemasInternals.h: $(srcdir)/include/libxml2/libxml/schemasInternals.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/schemasInternals.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/globals.h
$(RUBYLIBDIR)/include/libxml2/libxml/globals.h: $(srcdir)/include/libxml2/libxml/globals.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/globals.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/parser.h
$(RUBYLIBDIR)/include/libxml2/libxml/parser.h: $(srcdir)/include/libxml2/libxml/parser.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/parser.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/catalog.h
$(RUBYLIBDIR)/include/libxml2/libxml/catalog.h: $(srcdir)/include/libxml2/libxml/catalog.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/catalog.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/schematron.h
$(RUBYLIBDIR)/include/libxml2/libxml/schematron.h: $(srcdir)/include/libxml2/libxml/schematron.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/schematron.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/chvalid.h
$(RUBYLIBDIR)/include/libxml2/libxml/chvalid.h: $(srcdir)/include/libxml2/libxml/chvalid.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/chvalid.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlIO.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlIO.h: $(srcdir)/include/libxml2/libxml/xmlIO.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlIO.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/SAX2.h
$(RUBYLIBDIR)/include/libxml2/libxml/SAX2.h: $(srcdir)/include/libxml2/libxml/SAX2.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/SAX2.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/tree.h
$(RUBYLIBDIR)/include/libxml2/libxml/tree.h: $(srcdir)/include/libxml2/libxml/tree.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/tree.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/HTMLparser.h
$(RUBYLIBDIR)/include/libxml2/libxml/HTMLparser.h: $(srcdir)/include/libxml2/libxml/HTMLparser.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/HTMLparser.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/relaxng.h
$(RUBYLIBDIR)/include/libxml2/libxml/relaxng.h: $(srcdir)/include/libxml2/libxml/relaxng.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/relaxng.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlexports.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlexports.h: $(srcdir)/include/libxml2/libxml/xmlexports.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlexports.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlmodule.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlmodule.h: $(srcdir)/include/libxml2/libxml/xmlmodule.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlmodule.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/hash.h
$(RUBYLIBDIR)/include/libxml2/libxml/hash.h: $(srcdir)/include/libxml2/libxml/hash.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/hash.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/entities.h
$(RUBYLIBDIR)/include/libxml2/libxml/entities.h: $(srcdir)/include/libxml2/libxml/entities.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/entities.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlmemory.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlmemory.h: $(srcdir)/include/libxml2/libxml/xmlmemory.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlmemory.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/dict.h
$(RUBYLIBDIR)/include/libxml2/libxml/dict.h: $(srcdir)/include/libxml2/libxml/dict.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/dict.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/encoding.h
$(RUBYLIBDIR)/include/libxml2/libxml/encoding.h: $(srcdir)/include/libxml2/libxml/encoding.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/encoding.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/list.h
$(RUBYLIBDIR)/include/libxml2/libxml/list.h: $(srcdir)/include/libxml2/libxml/list.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/list.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xpointer.h
$(RUBYLIBDIR)/include/libxml2/libxml/xpointer.h: $(srcdir)/include/libxml2/libxml/xpointer.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xpointer.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlregexp.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlregexp.h: $(srcdir)/include/libxml2/libxml/xmlregexp.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlregexp.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/threads.h
$(RUBYLIBDIR)/include/libxml2/libxml/threads.h: $(srcdir)/include/libxml2/libxml/threads.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/threads.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xlink.h
$(RUBYLIBDIR)/include/libxml2/libxml/xlink.h: $(srcdir)/include/libxml2/libxml/xlink.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xlink.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/pattern.h
$(RUBYLIBDIR)/include/libxml2/libxml/pattern.h: $(srcdir)/include/libxml2/libxml/pattern.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/pattern.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlreader.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlreader.h: $(srcdir)/include/libxml2/libxml/xmlreader.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlreader.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/nanohttp.h
$(RUBYLIBDIR)/include/libxml2/libxml/nanohttp.h: $(srcdir)/include/libxml2/libxml/nanohttp.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/nanohttp.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/SAX.h
$(RUBYLIBDIR)/include/libxml2/libxml/SAX.h: $(srcdir)/include/libxml2/libxml/SAX.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/SAX.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/c14n.h
$(RUBYLIBDIR)/include/libxml2/libxml/c14n.h: $(srcdir)/include/libxml2/libxml/c14n.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/c14n.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlunicode.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlunicode.h: $(srcdir)/include/libxml2/libxml/xmlunicode.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlunicode.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/debugXML.h
$(RUBYLIBDIR)/include/libxml2/libxml/debugXML.h: $(srcdir)/include/libxml2/libxml/debugXML.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/debugXML.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xpathInternals.h
$(RUBYLIBDIR)/include/libxml2/libxml/xpathInternals.h: $(srcdir)/include/libxml2/libxml/xpathInternals.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xpathInternals.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/parserInternals.h
$(RUBYLIBDIR)/include/libxml2/libxml/parserInternals.h: $(srcdir)/include/libxml2/libxml/parserInternals.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/parserInternals.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/valid.h
$(RUBYLIBDIR)/include/libxml2/libxml/valid.h: $(srcdir)/include/libxml2/libxml/valid.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/valid.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlwriter.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlwriter.h: $(srcdir)/include/libxml2/libxml/xmlwriter.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlwriter.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xinclude.h
$(RUBYLIBDIR)/include/libxml2/libxml/xinclude.h: $(srcdir)/include/libxml2/libxml/xinclude.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xinclude.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlschemas.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlschemas.h: $(srcdir)/include/libxml2/libxml/xmlschemas.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlschemas.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlschemastypes.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlschemastypes.h: $(srcdir)/include/libxml2/libxml/xmlschemastypes.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlschemastypes.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlversion.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlversion.h: $(srcdir)/include/libxml2/libxml/xmlversion.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlversion.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xpath.h
$(RUBYLIBDIR)/include/libxml2/libxml/xpath.h: $(srcdir)/include/libxml2/libxml/xpath.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xpath.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/nanoftp.h
$(RUBYLIBDIR)/include/libxml2/libxml/nanoftp.h: $(srcdir)/include/libxml2/libxml/nanoftp.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/nanoftp.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxml2/libxml/xmlerror.h
$(RUBYLIBDIR)/include/libxml2/libxml/xmlerror.h: $(srcdir)/include/libxml2/libxml/xmlerror.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxml2/libxml/xmlerror.h $(@D)
pre-install-rb: $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libexslt.time
do-install-rb: $(RUBYLIBDIR)/include/libexslt/exsltexports.h
$(RUBYLIBDIR)/include/libexslt/exsltexports.h: $(srcdir)/include/libexslt/exsltexports.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libexslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libexslt/exsltexports.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libexslt/exslt.h
$(RUBYLIBDIR)/include/libexslt/exslt.h: $(srcdir)/include/libexslt/exslt.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libexslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libexslt/exslt.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libexslt/exsltconfig.h
$(RUBYLIBDIR)/include/libexslt/exsltconfig.h: $(srcdir)/include/libexslt/exsltconfig.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libexslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libexslt/exsltconfig.h $(@D)
pre-install-rb: $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
do-install-rb: $(RUBYLIBDIR)/include/libxslt/variables.h
$(RUBYLIBDIR)/include/libxslt/variables.h: $(srcdir)/include/libxslt/variables.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/variables.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/preproc.h
$(RUBYLIBDIR)/include/libxslt/preproc.h: $(srcdir)/include/libxslt/preproc.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/preproc.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/numbersInternals.h
$(RUBYLIBDIR)/include/libxslt/numbersInternals.h: $(srcdir)/include/libxslt/numbersInternals.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/numbersInternals.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/xsltutils.h
$(RUBYLIBDIR)/include/libxslt/xsltutils.h: $(srcdir)/include/libxslt/xsltutils.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/xsltutils.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/xsltconfig.h
$(RUBYLIBDIR)/include/libxslt/xsltconfig.h: $(srcdir)/include/libxslt/xsltconfig.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/xsltconfig.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/templates.h
$(RUBYLIBDIR)/include/libxslt/templates.h: $(srcdir)/include/libxslt/templates.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/templates.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/xsltexports.h
$(RUBYLIBDIR)/include/libxslt/xsltexports.h: $(srcdir)/include/libxslt/xsltexports.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/xsltexports.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/xsltInternals.h
$(RUBYLIBDIR)/include/libxslt/xsltInternals.h: $(srcdir)/include/libxslt/xsltInternals.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/xsltInternals.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/extra.h
$(RUBYLIBDIR)/include/libxslt/extra.h: $(srcdir)/include/libxslt/extra.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/extra.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/pattern.h
$(RUBYLIBDIR)/include/libxslt/pattern.h: $(srcdir)/include/libxslt/pattern.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/pattern.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/functions.h
$(RUBYLIBDIR)/include/libxslt/functions.h: $(srcdir)/include/libxslt/functions.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/functions.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/documents.h
$(RUBYLIBDIR)/include/libxslt/documents.h: $(srcdir)/include/libxslt/documents.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/documents.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/xslt.h
$(RUBYLIBDIR)/include/libxslt/xslt.h: $(srcdir)/include/libxslt/xslt.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/xslt.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/attributes.h
$(RUBYLIBDIR)/include/libxslt/attributes.h: $(srcdir)/include/libxslt/attributes.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/attributes.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/extensions.h
$(RUBYLIBDIR)/include/libxslt/extensions.h: $(srcdir)/include/libxslt/extensions.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/extensions.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/transform.h
$(RUBYLIBDIR)/include/libxslt/transform.h: $(srcdir)/include/libxslt/transform.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/transform.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/security.h
$(RUBYLIBDIR)/include/libxslt/security.h: $(srcdir)/include/libxslt/security.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/security.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/imports.h
$(RUBYLIBDIR)/include/libxslt/imports.h: $(srcdir)/include/libxslt/imports.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/imports.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/namespaces.h
$(RUBYLIBDIR)/include/libxslt/namespaces.h: $(srcdir)/include/libxslt/namespaces.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/namespaces.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/xsltlocale.h
$(RUBYLIBDIR)/include/libxslt/xsltlocale.h: $(srcdir)/include/libxslt/xsltlocale.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/xsltlocale.h $(@D)
do-install-rb: $(RUBYLIBDIR)/include/libxslt/keys.h
$(RUBYLIBDIR)/include/libxslt/keys.h: $(srcdir)/include/libxslt/keys.h $(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time
	$(Q) $(INSTALL_DATA) $(srcdir)/include/libxslt/keys.h $(@D)
pre-install-rb:
	$(Q1:0=@$(MAKE) -q do-install-rb || )$(ECHO1:0=echo) installing nokogiri libraries
$(TIMESTAMP_DIR)/.sitearchdir.-.nokogiri.time:
	$(Q) $(MAKEDIRS) $(@D) $(RUBYARCHDIR)
	$(Q) $(TOUCH) $@
$(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxml2.-.libxml.time:
	$(Q) $(MAKEDIRS) $(@D) $(RUBYLIBDIR)/include/libxml2/libxml
	$(Q) $(TOUCH) $@
$(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libexslt.time:
	$(Q) $(MAKEDIRS) $(@D) $(RUBYLIBDIR)/include/libexslt
	$(Q) $(TOUCH) $@
$(TIMESTAMP_DIR)/.sitelibdir.-.nokogiri.-.include.-.libxslt.time:
	$(Q) $(MAKEDIRS) $(@D) $(RUBYLIBDIR)/include/libxslt
	$(Q) $(TOUCH) $@

site-install: site-install-so site-install-rb
site-install-so: install-so
site-install-rb: install-rb

.SUFFIXES: .c .m .cc .mm .cxx .cpp .o .S

.cc.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $(CSRCFLAG)$<

.cc.S:
	$(ECHO) translating $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -S $(CSRCFLAG)$<

.mm.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $(CSRCFLAG)$<

.mm.S:
	$(ECHO) translating $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -S $(CSRCFLAG)$<

.cxx.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $(CSRCFLAG)$<

.cxx.S:
	$(ECHO) translating $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -S $(CSRCFLAG)$<

.cpp.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $(CSRCFLAG)$<

.cpp.S:
	$(ECHO) translating $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -S $(CSRCFLAG)$<

.c.o:
	$(ECHO) compiling $(<)
	$(Q) $(CC) $(INCFLAGS) $(CPPFLAGS) $(CFLAGS) $(COUTFLAG)$@ -c $(CSRCFLAG)$<

.c.S:
	$(ECHO) translating $(<)
	$(Q) $(CC) $(INCFLAGS) $(CPPFLAGS) $(CFLAGS) $(COUTFLAG)$@ -S $(CSRCFLAG)$<

.m.o:
	$(ECHO) compiling $(<)
	$(Q) $(CC) $(INCFLAGS) $(CPPFLAGS) $(CFLAGS) $(COUTFLAG)$@ -c $(CSRCFLAG)$<

.m.S:
	$(ECHO) translating $(<)
	$(Q) $(CC) $(INCFLAGS) $(CPPFLAGS) $(CFLAGS) $(COUTFLAG)$@ -S $(CSRCFLAG)$<

$(TARGET_SO): $(OBJS) Makefile
	$(ECHO) linking shared-object nokogiri/$(DLLIB)
	-$(Q)$(RM) $(@)
	$(Q) $(LDSHARED) -o $@ $(OBJS) $(LIBPATH) $(DLDFLAGS) $(LOCAL_LIBS) $(LIBS)



###
# -*-makefile-*-
# DO NOT DELETE

html_document.o: ./html_document.h ./nokogiri.h ./xml_libxml2_hacks.h
html_document.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
html_document.o: ./xml_node.h ./xml_text.h ./xml_cdata.h ./xml_attr.h
html_document.o: ./xml_processing_instruction.h ./xml_entity_reference.h
html_document.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
html_document.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
html_document.o: ./xml_entity_decl.h ./xml_xpath_context.h
html_document.o: ./xml_element_content.h ./xml_sax_parser_context.h
html_document.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
html_document.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
html_document.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
html_document.o: ./xml_relax_ng.h ./html_element_description.h
html_document.o: ./xml_namespace.h ./xml_encoding_handler.h
html_element_description.o: ./html_element_description.h ./nokogiri.h
html_element_description.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
html_element_description.o: ./html_entity_lookup.h ./html_document.h
html_element_description.o: ./xml_node.h ./xml_text.h ./xml_cdata.h
html_element_description.o: ./xml_attr.h ./xml_processing_instruction.h
html_element_description.o: ./xml_entity_reference.h
html_element_description.o: ./xml_document_fragment.h ./xml_comment.h
html_element_description.o: ./xml_node_set.h ./xml_dtd.h
html_element_description.o: ./xml_attribute_decl.h ./xml_element_decl.h
html_element_description.o: ./xml_entity_decl.h ./xml_xpath_context.h
html_element_description.o: ./xml_element_content.h
html_element_description.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
html_element_description.o: ./xml_sax_push_parser.h ./xml_reader.h
html_element_description.o: ./html_sax_parser_context.h
html_element_description.o: ./html_sax_push_parser.h ./xslt_stylesheet.h
html_element_description.o: ./xml_syntax_error.h ./xml_schema.h
html_element_description.o: ./xml_relax_ng.h ./xml_namespace.h
html_element_description.o: ./xml_encoding_handler.h
html_entity_lookup.o: ./html_entity_lookup.h ./nokogiri.h
html_entity_lookup.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
html_entity_lookup.o: ./html_document.h ./xml_node.h ./xml_text.h
html_entity_lookup.o: ./xml_cdata.h ./xml_attr.h
html_entity_lookup.o: ./xml_processing_instruction.h ./xml_entity_reference.h
html_entity_lookup.o: ./xml_document_fragment.h ./xml_comment.h
html_entity_lookup.o: ./xml_node_set.h ./xml_dtd.h ./xml_attribute_decl.h
html_entity_lookup.o: ./xml_element_decl.h ./xml_entity_decl.h
html_entity_lookup.o: ./xml_xpath_context.h ./xml_element_content.h
html_entity_lookup.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
html_entity_lookup.o: ./xml_sax_push_parser.h ./xml_reader.h
html_entity_lookup.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
html_entity_lookup.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
html_entity_lookup.o: ./xml_relax_ng.h ./html_element_description.h
html_entity_lookup.o: ./xml_namespace.h ./xml_encoding_handler.h
html_sax_parser_context.o: ./html_sax_parser_context.h ./nokogiri.h
html_sax_parser_context.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
html_sax_parser_context.o: ./html_entity_lookup.h ./html_document.h
html_sax_parser_context.o: ./xml_node.h ./xml_text.h ./xml_cdata.h
html_sax_parser_context.o: ./xml_attr.h ./xml_processing_instruction.h
html_sax_parser_context.o: ./xml_entity_reference.h ./xml_document_fragment.h
html_sax_parser_context.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
html_sax_parser_context.o: ./xml_attribute_decl.h ./xml_element_decl.h
html_sax_parser_context.o: ./xml_entity_decl.h ./xml_xpath_context.h
html_sax_parser_context.o: ./xml_element_content.h ./xml_sax_parser_context.h
html_sax_parser_context.o: ./xml_sax_parser.h ./xml_sax_push_parser.h
html_sax_parser_context.o: ./xml_reader.h ./html_sax_push_parser.h
html_sax_parser_context.o: ./xslt_stylesheet.h ./xml_syntax_error.h
html_sax_parser_context.o: ./xml_schema.h ./xml_relax_ng.h
html_sax_parser_context.o: ./html_element_description.h ./xml_namespace.h
html_sax_parser_context.o: ./xml_encoding_handler.h
html_sax_push_parser.o: ./html_sax_push_parser.h ./nokogiri.h
html_sax_push_parser.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
html_sax_push_parser.o: ./html_entity_lookup.h ./html_document.h ./xml_node.h
html_sax_push_parser.o: ./xml_text.h ./xml_cdata.h ./xml_attr.h
html_sax_push_parser.o: ./xml_processing_instruction.h
html_sax_push_parser.o: ./xml_entity_reference.h ./xml_document_fragment.h
html_sax_push_parser.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
html_sax_push_parser.o: ./xml_attribute_decl.h ./xml_element_decl.h
html_sax_push_parser.o: ./xml_entity_decl.h ./xml_xpath_context.h
html_sax_push_parser.o: ./xml_element_content.h ./xml_sax_parser_context.h
html_sax_push_parser.o: ./xml_sax_parser.h ./xml_sax_push_parser.h
html_sax_push_parser.o: ./xml_reader.h ./html_sax_parser_context.h
html_sax_push_parser.o: ./xslt_stylesheet.h ./xml_syntax_error.h
html_sax_push_parser.o: ./xml_schema.h ./xml_relax_ng.h
html_sax_push_parser.o: ./html_element_description.h ./xml_namespace.h
html_sax_push_parser.o: ./xml_encoding_handler.h
nokogiri.o: ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
nokogiri.o: ./html_entity_lookup.h ./html_document.h ./xml_node.h
nokogiri.o: ./xml_text.h ./xml_cdata.h ./xml_attr.h
nokogiri.o: ./xml_processing_instruction.h ./xml_entity_reference.h
nokogiri.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
nokogiri.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
nokogiri.o: ./xml_entity_decl.h ./xml_xpath_context.h ./xml_element_content.h
nokogiri.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
nokogiri.o: ./xml_sax_push_parser.h ./xml_reader.h
nokogiri.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
nokogiri.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
nokogiri.o: ./xml_relax_ng.h ./html_element_description.h ./xml_namespace.h
nokogiri.o: ./xml_encoding_handler.h
xml_attr.o: ./xml_attr.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h
xml_attr.o: ./xml_document.h ./html_entity_lookup.h ./html_document.h
xml_attr.o: ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_attr.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_attr.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
xml_attr.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
xml_attr.o: ./xml_entity_decl.h ./xml_xpath_context.h ./xml_element_content.h
xml_attr.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_attr.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_attr.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_attr.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_attr.o: ./xml_relax_ng.h ./html_element_description.h ./xml_namespace.h
xml_attr.o: ./xml_encoding_handler.h
xml_attribute_decl.o: ./xml_attribute_decl.h ./nokogiri.h
xml_attribute_decl.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
xml_attribute_decl.o: ./html_entity_lookup.h ./html_document.h ./xml_node.h
xml_attribute_decl.o: ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_attribute_decl.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_attribute_decl.o: ./xml_document_fragment.h ./xml_comment.h
xml_attribute_decl.o: ./xml_node_set.h ./xml_dtd.h ./xml_element_decl.h
xml_attribute_decl.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_attribute_decl.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_attribute_decl.o: ./xml_sax_parser.h ./xml_sax_push_parser.h
xml_attribute_decl.o: ./xml_reader.h ./html_sax_parser_context.h
xml_attribute_decl.o: ./html_sax_push_parser.h ./xslt_stylesheet.h
xml_attribute_decl.o: ./xml_syntax_error.h ./xml_schema.h ./xml_relax_ng.h
xml_attribute_decl.o: ./html_element_description.h ./xml_namespace.h
xml_attribute_decl.o: ./xml_encoding_handler.h
xml_cdata.o: ./xml_cdata.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h
xml_cdata.o: ./xml_document.h ./html_entity_lookup.h ./html_document.h
xml_cdata.o: ./xml_node.h ./xml_text.h ./xml_attr.h
xml_cdata.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_cdata.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
xml_cdata.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
xml_cdata.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_cdata.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_cdata.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xml_cdata.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_cdata.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_cdata.o: ./xml_relax_ng.h ./html_element_description.h ./xml_namespace.h
xml_cdata.o: ./xml_encoding_handler.h
xml_comment.o: ./xml_comment.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h
xml_comment.o: ./xml_document.h ./html_entity_lookup.h ./html_document.h
xml_comment.o: ./xml_node.h ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_comment.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_comment.o: ./xml_document_fragment.h ./xml_node_set.h ./xml_dtd.h
xml_comment.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_comment.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_comment.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_comment.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xml_comment.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_comment.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_comment.o: ./xml_relax_ng.h ./html_element_description.h
xml_comment.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_document.o: ./xml_document.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_document.o: ./xml_io.h ./html_entity_lookup.h ./html_document.h
xml_document.o: ./xml_node.h ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_document.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_document.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
xml_document.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
xml_document.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_document.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_document.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xml_document.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_document.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_document.o: ./xml_relax_ng.h ./html_element_description.h
xml_document.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_document_fragment.o: ./xml_document_fragment.h ./nokogiri.h
xml_document_fragment.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
xml_document_fragment.o: ./html_entity_lookup.h ./html_document.h
xml_document_fragment.o: ./xml_node.h ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_document_fragment.o: ./xml_processing_instruction.h
xml_document_fragment.o: ./xml_entity_reference.h ./xml_comment.h
xml_document_fragment.o: ./xml_node_set.h ./xml_dtd.h ./xml_attribute_decl.h
xml_document_fragment.o: ./xml_element_decl.h ./xml_entity_decl.h
xml_document_fragment.o: ./xml_xpath_context.h ./xml_element_content.h
xml_document_fragment.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_document_fragment.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_document_fragment.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_document_fragment.o: ./xslt_stylesheet.h ./xml_syntax_error.h
xml_document_fragment.o: ./xml_schema.h ./xml_relax_ng.h
xml_document_fragment.o: ./html_element_description.h ./xml_namespace.h
xml_document_fragment.o: ./xml_encoding_handler.h
xml_dtd.o: ./xml_dtd.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h
xml_dtd.o: ./xml_document.h ./html_entity_lookup.h ./html_document.h
xml_dtd.o: ./xml_node.h ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_dtd.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_dtd.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
xml_dtd.o: ./xml_attribute_decl.h ./xml_element_decl.h ./xml_entity_decl.h
xml_dtd.o: ./xml_xpath_context.h ./xml_element_content.h
xml_dtd.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_dtd.o: ./xml_sax_push_parser.h ./xml_reader.h ./html_sax_parser_context.h
xml_dtd.o: ./html_sax_push_parser.h ./xslt_stylesheet.h ./xml_syntax_error.h
xml_dtd.o: ./xml_schema.h ./xml_relax_ng.h ./html_element_description.h
xml_dtd.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_element_content.o: ./xml_element_content.h ./nokogiri.h
xml_element_content.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
xml_element_content.o: ./html_entity_lookup.h ./html_document.h ./xml_node.h
xml_element_content.o: ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_element_content.o: ./xml_processing_instruction.h
xml_element_content.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_element_content.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_element_content.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_element_content.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_element_content.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_element_content.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_element_content.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_element_content.o: ./xslt_stylesheet.h ./xml_syntax_error.h
xml_element_content.o: ./xml_schema.h ./xml_relax_ng.h
xml_element_content.o: ./html_element_description.h ./xml_namespace.h
xml_element_content.o: ./xml_encoding_handler.h
xml_element_decl.o: ./xml_element_decl.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_element_decl.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xml_element_decl.o: ./html_document.h ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_element_decl.o: ./xml_attr.h ./xml_processing_instruction.h
xml_element_decl.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_element_decl.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_element_decl.o: ./xml_attribute_decl.h ./xml_entity_decl.h
xml_element_decl.o: ./xml_xpath_context.h ./xml_element_content.h
xml_element_decl.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_element_decl.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_element_decl.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_element_decl.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_element_decl.o: ./xml_relax_ng.h ./html_element_description.h
xml_element_decl.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_encoding_handler.o: ./xml_encoding_handler.h ./nokogiri.h
xml_encoding_handler.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
xml_encoding_handler.o: ./html_entity_lookup.h ./html_document.h ./xml_node.h
xml_encoding_handler.o: ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_encoding_handler.o: ./xml_processing_instruction.h
xml_encoding_handler.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_encoding_handler.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_encoding_handler.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_encoding_handler.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_encoding_handler.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_encoding_handler.o: ./xml_sax_parser.h ./xml_sax_push_parser.h
xml_encoding_handler.o: ./xml_reader.h ./html_sax_parser_context.h
xml_encoding_handler.o: ./html_sax_push_parser.h ./xslt_stylesheet.h
xml_encoding_handler.o: ./xml_syntax_error.h ./xml_schema.h ./xml_relax_ng.h
xml_encoding_handler.o: ./html_element_description.h ./xml_namespace.h
xml_entity_decl.o: ./xml_entity_decl.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_entity_decl.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xml_entity_decl.o: ./html_document.h ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_entity_decl.o: ./xml_attr.h ./xml_processing_instruction.h
xml_entity_decl.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_entity_decl.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_entity_decl.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_entity_decl.o: ./xml_xpath_context.h ./xml_element_content.h
xml_entity_decl.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_entity_decl.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_entity_decl.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_entity_decl.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_entity_decl.o: ./xml_relax_ng.h ./html_element_description.h
xml_entity_decl.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_entity_reference.o: ./xml_entity_reference.h ./nokogiri.h
xml_entity_reference.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
xml_entity_reference.o: ./html_entity_lookup.h ./html_document.h ./xml_node.h
xml_entity_reference.o: ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_entity_reference.o: ./xml_processing_instruction.h
xml_entity_reference.o: ./xml_document_fragment.h ./xml_comment.h
xml_entity_reference.o: ./xml_node_set.h ./xml_dtd.h ./xml_attribute_decl.h
xml_entity_reference.o: ./xml_element_decl.h ./xml_entity_decl.h
xml_entity_reference.o: ./xml_xpath_context.h ./xml_element_content.h
xml_entity_reference.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_entity_reference.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_entity_reference.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_entity_reference.o: ./xslt_stylesheet.h ./xml_syntax_error.h
xml_entity_reference.o: ./xml_schema.h ./xml_relax_ng.h
xml_entity_reference.o: ./html_element_description.h ./xml_namespace.h
xml_entity_reference.o: ./xml_encoding_handler.h
xml_io.o: ./xml_io.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_document.h
xml_io.o: ./html_entity_lookup.h ./html_document.h ./xml_node.h ./xml_text.h
xml_io.o: ./xml_cdata.h ./xml_attr.h ./xml_processing_instruction.h
xml_io.o: ./xml_entity_reference.h ./xml_document_fragment.h ./xml_comment.h
xml_io.o: ./xml_node_set.h ./xml_dtd.h ./xml_attribute_decl.h
xml_io.o: ./xml_element_decl.h ./xml_entity_decl.h ./xml_xpath_context.h
xml_io.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_io.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xml_io.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_io.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_io.o: ./xml_relax_ng.h ./html_element_description.h ./xml_namespace.h
xml_io.o: ./xml_encoding_handler.h
xml_namespace.o: ./xml_namespace.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_namespace.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xml_namespace.o: ./html_document.h ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_namespace.o: ./xml_attr.h ./xml_processing_instruction.h
xml_namespace.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_namespace.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_namespace.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_namespace.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_namespace.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_namespace.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xml_namespace.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_namespace.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_namespace.o: ./xml_relax_ng.h ./html_element_description.h
xml_namespace.o: ./xml_encoding_handler.h
xml_node.o: ./xml_node.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h
xml_node.o: ./xml_document.h ./html_entity_lookup.h ./html_document.h
xml_node.o: ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_node.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_node.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
xml_node.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
xml_node.o: ./xml_entity_decl.h ./xml_xpath_context.h ./xml_element_content.h
xml_node.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_node.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_node.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_node.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_node.o: ./xml_relax_ng.h ./html_element_description.h ./xml_namespace.h
xml_node.o: ./xml_encoding_handler.h
xml_node_set.o: ./xml_node_set.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_node_set.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xml_node_set.o: ./html_document.h ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_node_set.o: ./xml_attr.h ./xml_processing_instruction.h
xml_node_set.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_node_set.o: ./xml_comment.h ./xml_dtd.h ./xml_attribute_decl.h
xml_node_set.o: ./xml_element_decl.h ./xml_entity_decl.h
xml_node_set.o: ./xml_xpath_context.h ./xml_element_content.h
xml_node_set.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_node_set.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_node_set.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_node_set.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_node_set.o: ./xml_relax_ng.h ./html_element_description.h
xml_node_set.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_processing_instruction.o: ./xml_processing_instruction.h ./nokogiri.h
xml_processing_instruction.o: ./xml_libxml2_hacks.h ./xml_io.h
xml_processing_instruction.o: ./xml_document.h ./html_entity_lookup.h
xml_processing_instruction.o: ./html_document.h ./xml_node.h ./xml_text.h
xml_processing_instruction.o: ./xml_cdata.h ./xml_attr.h
xml_processing_instruction.o: ./xml_entity_reference.h
xml_processing_instruction.o: ./xml_document_fragment.h ./xml_comment.h
xml_processing_instruction.o: ./xml_node_set.h ./xml_dtd.h
xml_processing_instruction.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_processing_instruction.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_processing_instruction.o: ./xml_element_content.h
xml_processing_instruction.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_processing_instruction.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_processing_instruction.o: ./html_sax_parser_context.h
xml_processing_instruction.o: ./html_sax_push_parser.h ./xslt_stylesheet.h
xml_processing_instruction.o: ./xml_syntax_error.h ./xml_schema.h
xml_processing_instruction.o: ./xml_relax_ng.h ./html_element_description.h
xml_processing_instruction.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_reader.o: ./xml_reader.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h
xml_reader.o: ./xml_document.h ./html_entity_lookup.h ./html_document.h
xml_reader.o: ./xml_node.h ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_reader.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_reader.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
xml_reader.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
xml_reader.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_reader.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_reader.o: ./xml_sax_parser.h ./xml_sax_push_parser.h
xml_reader.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_reader.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_reader.o: ./xml_relax_ng.h ./html_element_description.h ./xml_namespace.h
xml_reader.o: ./xml_encoding_handler.h
xml_relax_ng.o: ./xml_relax_ng.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_relax_ng.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xml_relax_ng.o: ./html_document.h ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_relax_ng.o: ./xml_attr.h ./xml_processing_instruction.h
xml_relax_ng.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_relax_ng.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_relax_ng.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_relax_ng.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_relax_ng.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_relax_ng.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xml_relax_ng.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_relax_ng.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_relax_ng.o: ./html_element_description.h ./xml_namespace.h
xml_relax_ng.o: ./xml_encoding_handler.h
xml_sax_parser.o: ./xml_sax_parser.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_sax_parser.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xml_sax_parser.o: ./html_document.h ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_sax_parser.o: ./xml_attr.h ./xml_processing_instruction.h
xml_sax_parser.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_sax_parser.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_sax_parser.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_sax_parser.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_sax_parser.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_sax_parser.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_sax_parser.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_sax_parser.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_sax_parser.o: ./xml_relax_ng.h ./html_element_description.h
xml_sax_parser.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_sax_parser_context.o: ./xml_sax_parser_context.h ./nokogiri.h
xml_sax_parser_context.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
xml_sax_parser_context.o: ./html_entity_lookup.h ./html_document.h
xml_sax_parser_context.o: ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_sax_parser_context.o: ./xml_attr.h ./xml_processing_instruction.h
xml_sax_parser_context.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_sax_parser_context.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_sax_parser_context.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_sax_parser_context.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_sax_parser_context.o: ./xml_element_content.h ./xml_sax_parser.h
xml_sax_parser_context.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_sax_parser_context.o: ./html_sax_parser_context.h
xml_sax_parser_context.o: ./html_sax_push_parser.h ./xslt_stylesheet.h
xml_sax_parser_context.o: ./xml_syntax_error.h ./xml_schema.h
xml_sax_parser_context.o: ./xml_relax_ng.h ./html_element_description.h
xml_sax_parser_context.o: ./xml_namespace.h ./xml_encoding_handler.h
xml_sax_push_parser.o: ./xml_sax_push_parser.h ./nokogiri.h
xml_sax_push_parser.o: ./xml_libxml2_hacks.h ./xml_io.h ./xml_document.h
xml_sax_push_parser.o: ./html_entity_lookup.h ./html_document.h ./xml_node.h
xml_sax_push_parser.o: ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_sax_push_parser.o: ./xml_processing_instruction.h
xml_sax_push_parser.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_sax_push_parser.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_sax_push_parser.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_sax_push_parser.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_sax_push_parser.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_sax_push_parser.o: ./xml_sax_parser.h ./xml_reader.h
xml_sax_push_parser.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_sax_push_parser.o: ./xslt_stylesheet.h ./xml_syntax_error.h
xml_sax_push_parser.o: ./xml_schema.h ./xml_relax_ng.h
xml_sax_push_parser.o: ./html_element_description.h ./xml_namespace.h
xml_sax_push_parser.o: ./xml_encoding_handler.h
xml_schema.o: ./xml_schema.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h
xml_schema.o: ./xml_document.h ./html_entity_lookup.h ./html_document.h
xml_schema.o: ./xml_node.h ./xml_text.h ./xml_cdata.h ./xml_attr.h
xml_schema.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_schema.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
xml_schema.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
xml_schema.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_schema.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_schema.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xml_schema.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_schema.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_relax_ng.h
xml_schema.o: ./html_element_description.h ./xml_namespace.h
xml_schema.o: ./xml_encoding_handler.h
xml_syntax_error.o: ./xml_syntax_error.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_syntax_error.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xml_syntax_error.o: ./html_document.h ./xml_node.h ./xml_text.h ./xml_cdata.h
xml_syntax_error.o: ./xml_attr.h ./xml_processing_instruction.h
xml_syntax_error.o: ./xml_entity_reference.h ./xml_document_fragment.h
xml_syntax_error.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xml_syntax_error.o: ./xml_attribute_decl.h ./xml_element_decl.h
xml_syntax_error.o: ./xml_entity_decl.h ./xml_xpath_context.h
xml_syntax_error.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_syntax_error.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xml_syntax_error.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_syntax_error.o: ./xslt_stylesheet.h ./xml_schema.h ./xml_relax_ng.h
xml_syntax_error.o: ./html_element_description.h ./xml_namespace.h
xml_syntax_error.o: ./xml_encoding_handler.h
xml_text.o: ./xml_text.h ./nokogiri.h ./xml_libxml2_hacks.h ./xml_io.h
xml_text.o: ./xml_document.h ./html_entity_lookup.h ./html_document.h
xml_text.o: ./xml_node.h ./xml_cdata.h ./xml_attr.h
xml_text.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_text.o: ./xml_document_fragment.h ./xml_comment.h ./xml_node_set.h
xml_text.o: ./xml_dtd.h ./xml_attribute_decl.h ./xml_element_decl.h
xml_text.o: ./xml_entity_decl.h ./xml_xpath_context.h ./xml_element_content.h
xml_text.o: ./xml_sax_parser_context.h ./xml_sax_parser.h
xml_text.o: ./xml_sax_push_parser.h ./xml_reader.h
xml_text.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xml_text.o: ./xslt_stylesheet.h ./xml_syntax_error.h ./xml_schema.h
xml_text.o: ./xml_relax_ng.h ./html_element_description.h ./xml_namespace.h
xml_text.o: ./xml_encoding_handler.h
xml_xpath_context.o: ./xml_xpath_context.h ./nokogiri.h ./xml_libxml2_hacks.h
xml_xpath_context.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xml_xpath_context.o: ./html_document.h ./xml_node.h ./xml_text.h
xml_xpath_context.o: ./xml_cdata.h ./xml_attr.h
xml_xpath_context.o: ./xml_processing_instruction.h ./xml_entity_reference.h
xml_xpath_context.o: ./xml_document_fragment.h ./xml_comment.h
xml_xpath_context.o: ./xml_node_set.h ./xml_dtd.h ./xml_attribute_decl.h
xml_xpath_context.o: ./xml_element_decl.h ./xml_entity_decl.h
xml_xpath_context.o: ./xml_element_content.h ./xml_sax_parser_context.h
xml_xpath_context.o: ./xml_sax_parser.h ./xml_sax_push_parser.h
xml_xpath_context.o: ./xml_reader.h ./html_sax_parser_context.h
xml_xpath_context.o: ./html_sax_push_parser.h ./xslt_stylesheet.h
xml_xpath_context.o: ./xml_syntax_error.h ./xml_schema.h ./xml_relax_ng.h
xml_xpath_context.o: ./html_element_description.h ./xml_namespace.h
xml_xpath_context.o: ./xml_encoding_handler.h
xslt_stylesheet.o: ./xslt_stylesheet.h ./nokogiri.h ./xml_libxml2_hacks.h
xslt_stylesheet.o: ./xml_io.h ./xml_document.h ./html_entity_lookup.h
xslt_stylesheet.o: ./html_document.h ./xml_node.h ./xml_text.h ./xml_cdata.h
xslt_stylesheet.o: ./xml_attr.h ./xml_processing_instruction.h
xslt_stylesheet.o: ./xml_entity_reference.h ./xml_document_fragment.h
xslt_stylesheet.o: ./xml_comment.h ./xml_node_set.h ./xml_dtd.h
xslt_stylesheet.o: ./xml_attribute_decl.h ./xml_element_decl.h
xslt_stylesheet.o: ./xml_entity_decl.h ./xml_xpath_context.h
xslt_stylesheet.o: ./xml_element_content.h ./xml_sax_parser_context.h
xslt_stylesheet.o: ./xml_sax_parser.h ./xml_sax_push_parser.h ./xml_reader.h
xslt_stylesheet.o: ./html_sax_parser_context.h ./html_sax_push_parser.h
xslt_stylesheet.o: ./xml_syntax_error.h ./xml_schema.h ./xml_relax_ng.h
xslt_stylesheet.o: ./html_element_description.h ./xml_namespace.h
xslt_stylesheet.o: ./xml_encoding_handler.h

all: clean-ports
clean-ports: $(DLLIB)
	-$(Q)$(RUBY) $(srcdir)/extconf.rb --clean --enable-static

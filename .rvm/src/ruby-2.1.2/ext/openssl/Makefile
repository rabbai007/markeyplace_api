
SHELL = /bin/sh

# V=0 quiet, V=1 verbose.  other values don't work.
V = 0
Q1 = $(V:1=)
Q = $(Q1:0=@)
ECHO1 = $(V:1=@:)
ECHO = $(ECHO1:0=@echo)

#### Start of system configuration section. ####
top_srcdir = $(topdir)/.
srcdir = $(top_srcdir)/ext/openssl
topdir = ../..
hdrdir = $(top_srcdir)/include
arch_hdrdir = $(extout)/include/$(arch)
PATH_SEPARATOR = :
VPATH = $(srcdir):$(arch_hdrdir)/ruby:$(hdrdir)/ruby
RUBYLIB =
RUBYOPT = -
prefix = $(DESTDIR)/home/fsgapp/.rvm/rubies/ruby-2.1.2
rubysitearchprefix = $(rubylibprefix)/$(sitearch)
rubyarchprefix = $(rubylibprefix)/$(arch)
rubylibprefix = $(libdir)/$(RUBY_BASE_NAME)
exec_prefix = $(prefix)
vendorarchhdrdir = $(vendorhdrdir)/$(sitearch)
sitearchhdrdir = $(sitehdrdir)/$(sitearch)
rubyarchhdrdir = $(rubyhdrdir)/$(arch)
vendorhdrdir = $(rubyhdrdir)/vendor_ruby
sitehdrdir = $(rubyhdrdir)/site_ruby
rubyhdrdir = $(includedir)/$(RUBY_VERSION_NAME)
vendorarchdir = $(vendorlibdir)/$(sitearch)
vendorlibdir = $(vendordir)/$(ruby_version)
vendordir = $(rubylibprefix)/vendor_ruby
sitearchdir = $(sitelibdir)/$(sitearch)
sitelibdir = $(sitedir)/$(ruby_version)
sitedir = $(rubylibprefix)/site_ruby
rubyarchdir = $(rubylibdir)/$(arch)
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
localstatedir = $(prefix)/var
sharedstatedir = $(prefix)/com
sysconfdir = $(prefix)/etc
datadir = $(datarootdir)
datarootdir = $(prefix)/share
libexecdir = $(exec_prefix)/libexec
sbindir = $(exec_prefix)/sbin
bindir = $(exec_prefix)/bin
archdir = $(rubyarchdir)


CC = gcc
CXX = g++
LIBRUBY = $(LIBRUBY_SO)
LIBRUBY_A = lib$(RUBY_SO_NAME)-static.a
LIBRUBYARG_SHARED = -Wl,-R -Wl,$(libdir) -L$(libdir) -l$(RUBY_SO_NAME)
LIBRUBYARG_STATIC = -Wl,-R -Wl,$(libdir) -L$(libdir) -l$(RUBY_SO_NAME)-static
empty =
OUTFLAG = -o $(empty)
COUTFLAG = -o $(empty)

RUBY_EXTCONF_H = extconf.h
cflags   =  $(optflags) $(debugflags) $(warnflags)
optflags = -O3 -fno-fast-math
debugflags = -ggdb3
warnflags = -Wall -Wextra -Wno-unused-parameter -Wno-parentheses -Wno-long-long -Wno-missing-field-initializers -Wunused-variable -Wpointer-arith -Wwrite-strings -Wdeclaration-after-statement -Wimplicit-function-declaration
CCDLFLAGS = -fPIC
CFLAGS   = $(CCDLFLAGS) $(cflags)  -fPIC -I/usr/kerberos/include $(ARCH_FLAG)
INCFLAGS = -I. -I$(arch_hdrdir) -I$(hdrdir) -I$(srcdir)
DEFS     = 
CPPFLAGS = -DRUBY_EXTCONF_H=\"$(RUBY_EXTCONF_H)\"  $(DEFS) $(cppflags)
CXXFLAGS = $(CCDLFLAGS) $(cxxflags) $(ARCH_FLAG)
ldflags  = -L. -fstack-protector -rdynamic -Wl,-export-dynamic -L/usr/kerberos/lib64
dldflags =  
ARCH_FLAG = 
DLDFLAGS = $(ldflags) $(dldflags) $(ARCH_FLAG)
LDSHARED = $(CC) -shared
LDSHAREDXX = $(CXX) -shared
AR = ar
EXEEXT = 

RUBY_INSTALL_NAME = ruby
RUBY_SO_NAME = ruby
RUBYW_INSTALL_NAME = 
RUBY_VERSION_NAME = $(RUBY_BASE_NAME)-$(ruby_version)
RUBYW_BASE_NAME = rubyw
RUBY_BASE_NAME = ruby

arch = x86_64-linux
sitearch = $(arch)
ruby_version = 2.1.0
ruby = $(topdir)/miniruby -I'$(topdir)' -I'$(top_srcdir)/lib' -I'$(extout)/$(arch)' -I'$(extout)/common'
RUBY = $(ruby)
ruby_headers = $(hdrdir)/ruby.h $(hdrdir)/ruby/ruby.h $(hdrdir)/ruby/defines.h $(hdrdir)/ruby/missing.h $(hdrdir)/ruby/intern.h $(hdrdir)/ruby/st.h $(hdrdir)/ruby/subst.h $(arch_hdrdir)/ruby/config.h $(RUBY_EXTCONF_H)

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
THREAD_MODEL = pthread

libpath = . $(topdir)
LIBPATH =  -L. -L$(topdir)
DEFFILE = 

CLEANFILES = mkmf.log
DISTCLEANFILES = 
DISTCLEANDIRS = 

extout = $(topdir)/.ext
extout_prefix = $(extout)$(target_prefix)/
target_prefix = 
LOCAL_LIBS = 
LIBS = $(LIBRUBYARG_SHARED)  -lssl -lcrypto -ldl -lz -lpthread -lrt -ldl -lcrypt -lm   -lc
ORIG_SRCS = ossl_asn1.c ossl_engine.c ossl_ns_spki.c ossl_pkey_ec.c ossl.c ossl_bio.c ossl_pkcs12.c ossl_x509store.c ossl_pkcs5.c ossl_pkey_dh.c ossl_x509attr.c openssl_missing.c ossl_pkey.c ossl_ssl.c ossl_ocsp.c ossl_cipher.c ossl_x509revoked.c ossl_x509req.c ossl_x509crl.c ossl_pkcs7.c ossl_digest.c ossl_x509ext.c ossl_config.c ossl_x509.c ossl_rand.c ossl_x509cert.c ossl_pkey_rsa.c ossl_pkey_dsa.c ossl_x509name.c ossl_ssl_session.c ossl_bn.c ossl_hmac.c
SRCS = $(ORIG_SRCS) 
OBJS = ossl_asn1.o ossl_engine.o ossl_ns_spki.o ossl_pkey_ec.o ossl.o ossl_bio.o ossl_pkcs12.o ossl_x509store.o ossl_pkcs5.o ossl_pkey_dh.o ossl_x509attr.o openssl_missing.o ossl_pkey.o ossl_ssl.o ossl_ocsp.o ossl_cipher.o ossl_x509revoked.o ossl_x509req.o ossl_x509crl.o ossl_pkcs7.o ossl_digest.o ossl_x509ext.o ossl_config.o ossl_x509.o ossl_rand.o ossl_x509cert.o ossl_pkey_rsa.o ossl_pkey_dsa.o ossl_x509name.o ossl_ssl_session.o ossl_bn.o ossl_hmac.o
HDRS = $(srcdir)/ossl.h $(srcdir)/ossl_ocsp.h $(srcdir)/ossl_bn.h $(srcdir)/ossl_hmac.h $(srcdir)/ossl_pkcs5.h $(srcdir)/ossl_pkey.h $(srcdir)/ossl_pkcs12.h $(srcdir)/ossl_digest.h $(srcdir)/ossl_cipher.h $(srcdir)/ossl_rand.h $(srcdir)/ossl_ns_spki.h $(srcdir)/ossl_engine.h $(srcdir)/ossl_x509.h $(srcdir)/ossl_version.h $(srcdir)/openssl_missing.h $(srcdir)/ossl_pkcs7.h $(srcdir)/ossl_ssl.h $(srcdir)/extconf.h $(srcdir)/ruby_missing.h $(srcdir)/ossl_asn1.h $(srcdir)/ossl_bio.h $(srcdir)/ossl_config.h
TARGET = openssl
TARGET_NAME = openssl
TARGET_ENTRY = Init_$(TARGET_NAME)
DLLIB = $(TARGET).so
EXTSTATIC = 
STATIC_LIB = 

TIMESTAMP_DIR = $(extout)/.timestamp
BINDIR        = $(extout)/bin
RUBYCOMMONDIR = $(extout)/common
RUBYLIBDIR    = $(RUBYCOMMONDIR)$(target_prefix)
RUBYARCHDIR   = $(extout)/$(arch)$(target_prefix)
HDRDIR        = $(extout)/include/ruby$(target_prefix)
ARCHHDRDIR    = $(extout)/include/$(arch)/ruby$(target_prefix)

TARGET_SO     = $(RUBYARCHDIR)/$(DLLIB)
CLEANLIBS     = $(RUBYARCHDIR)/$(TARGET).so 
CLEANOBJS     = *.o  *.bak

all:    install
static: all
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

install-so: $(RUBYARCHDIR)/$(DLLIB)
clean-so::
	-$(Q)$(RM) $(RUBYARCHDIR)/$(DLLIB)
	-$(Q)$(RMDIRS) $(RUBYARCHDIR) 2> /dev/null || true
clean-static::
	-$(Q)$(RM) $(STATIC_LIB)
install-rb: pre-install-rb install-rb-default
install-rb-default: pre-install-rb-default
pre-install-rb: Makefile
pre-install-rb-default: Makefile
pre-install-rb-default: $(TIMESTAMP_DIR)/.RUBYLIBDIR.time
install-rb-default: $(RUBYLIBDIR)/openssl.rb
$(RUBYLIBDIR)/openssl.rb: $(srcdir)/lib/openssl.rb $(TIMESTAMP_DIR)/.RUBYLIBDIR.time
	$(Q) $(COPY) $(srcdir)/lib/openssl.rb $(@D)
clean-rb-default::
	-$(Q)$(RM) $(RUBYLIBDIR)/openssl.rb
pre-install-rb-default: $(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time
install-rb-default: $(RUBYLIBDIR)/openssl/buffering.rb
$(RUBYLIBDIR)/openssl/buffering.rb: $(srcdir)/lib/openssl/buffering.rb $(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time
	$(Q) $(COPY) $(srcdir)/lib/openssl/buffering.rb $(@D)
clean-rb-default::
	-$(Q)$(RM) $(RUBYLIBDIR)/openssl/buffering.rb
install-rb-default: $(RUBYLIBDIR)/openssl/ssl.rb
$(RUBYLIBDIR)/openssl/ssl.rb: $(srcdir)/lib/openssl/ssl.rb $(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time
	$(Q) $(COPY) $(srcdir)/lib/openssl/ssl.rb $(@D)
clean-rb-default::
	-$(Q)$(RM) $(RUBYLIBDIR)/openssl/ssl.rb
install-rb-default: $(RUBYLIBDIR)/openssl/config.rb
$(RUBYLIBDIR)/openssl/config.rb: $(srcdir)/lib/openssl/config.rb $(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time
	$(Q) $(COPY) $(srcdir)/lib/openssl/config.rb $(@D)
clean-rb-default::
	-$(Q)$(RM) $(RUBYLIBDIR)/openssl/config.rb
install-rb-default: $(RUBYLIBDIR)/openssl/x509.rb
$(RUBYLIBDIR)/openssl/x509.rb: $(srcdir)/lib/openssl/x509.rb $(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time
	$(Q) $(COPY) $(srcdir)/lib/openssl/x509.rb $(@D)
clean-rb-default::
	-$(Q)$(RM) $(RUBYLIBDIR)/openssl/x509.rb
install-rb-default: $(RUBYLIBDIR)/openssl/bn.rb
$(RUBYLIBDIR)/openssl/bn.rb: $(srcdir)/lib/openssl/bn.rb $(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time
	$(Q) $(COPY) $(srcdir)/lib/openssl/bn.rb $(@D)
clean-rb-default::
	-$(Q)$(RM) $(RUBYLIBDIR)/openssl/bn.rb
install-rb-default: $(RUBYLIBDIR)/openssl/cipher.rb
$(RUBYLIBDIR)/openssl/cipher.rb: $(srcdir)/lib/openssl/cipher.rb $(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time
	$(Q) $(COPY) $(srcdir)/lib/openssl/cipher.rb $(@D)
clean-rb-default::
	-$(Q)$(RM) $(RUBYLIBDIR)/openssl/cipher.rb
install-rb-default: $(RUBYLIBDIR)/openssl/digest.rb
$(RUBYLIBDIR)/openssl/digest.rb: $(srcdir)/lib/openssl/digest.rb $(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time
	$(Q) $(COPY) $(srcdir)/lib/openssl/digest.rb $(@D)
clean-rb-default::
	-$(Q)$(RM) $(RUBYLIBDIR)/openssl/digest.rb
pre-install-rb-default:
	$(ECHO) installing default openssl libraries
clean-rb-default::
	-$(Q)$(RMDIRS) $(RUBYLIBDIR)/openssl 2> /dev/null || true
	-$(Q)$(RMDIRS) $(RUBYLIBDIR) 2> /dev/null || true
$(TIMESTAMP_DIR)/.RUBYARCHDIR.time:
	$(Q) $(MAKEDIRS) $(@D) $(RUBYARCHDIR)
	$(Q) $(TOUCH) $@
$(TIMESTAMP_DIR)/.RUBYLIBDIR.time:
	$(Q) $(MAKEDIRS) $(@D) $(RUBYLIBDIR)
	$(Q) $(TOUCH) $@
$(TIMESTAMP_DIR)/.RUBYLIBDIR.-.openssl.time:
	$(Q) $(MAKEDIRS) $(@D) $(RUBYLIBDIR)/openssl
	$(Q) $(TOUCH) $@

site-install: site-install-so site-install-rb
site-install-so: install-so
site-install-rb: install-rb

.SUFFIXES: .c .m .cc .mm .cxx .cpp .C .o

.cc.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $<

.mm.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $<

.cxx.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $<

.cpp.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $<

.C.o:
	$(ECHO) compiling $(<)
	$(Q) $(CXX) $(INCFLAGS) $(CPPFLAGS) $(CXXFLAGS) $(COUTFLAG)$@ -c $<

.c.o:
	$(ECHO) compiling $(<)
	$(Q) $(CC) $(INCFLAGS) $(CPPFLAGS) $(CFLAGS) $(COUTFLAG)$@ -c $<

.m.o:
	$(ECHO) compiling $(<)
	$(Q) $(CC) $(INCFLAGS) $(CPPFLAGS) $(CFLAGS) $(COUTFLAG)$@ -c $<

$(RUBYARCHDIR)/$(DLLIB): $(OBJS) Makefile $(TIMESTAMP_DIR)/.RUBYARCHDIR.time
	$(ECHO) linking shared-object $(DLLIB)
	-$(Q)$(RM) $(@)
	$(Q) $(LDSHARED) -o $@ $(OBJS) $(LIBPATH) $(DLDFLAGS) $(LOCAL_LIBS) $(LIBS)



###
$(OBJS): $(RUBY_EXTCONF_H)

$(OBJS): $(HDRS) $(ruby_headers) \
  $(hdrdir)/ruby/io.h \
  $(hdrdir)/ruby/encoding.h \
  $(hdrdir)/ruby/oniguruma.h \
  $(hdrdir)/ruby/thread.h
ossl.o: $(top_srcdir)/thread_native.h $(top_srcdir)/thread_$(THREAD_MODEL).h

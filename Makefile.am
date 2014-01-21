
# gnulib-tool --lgpl=2 --libtool --with-tests --local-dir=local --import regex 
ACLOCAL_AMFLAGS = -I m4
SUBDIRS = lib . tests
AM_CPPFLAGS = -D_REGEX_RE_COMP

EXTRA_DIST = m4/gnulib-cache.m4 m4/gnulib-tool.m4 local/m4/regex.m4.diff
dist_doc_DATA = COPYING.LESSERv2 README NEWS ChangeLog

lib_LTLIBRARIES = libregex.la

libregex_la_SOURCES = regex.def
libregex_la_LIBADD = lib/libgnu.la
libregex_la_LDFLAGS = -no-undefined -version-info 1:0:0 \
	-export-symbols $(srcdir)/regex.def

include_HEADERS = lib/regex.h


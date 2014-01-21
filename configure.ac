AC_PREREQ(2.63)
AC_INIT([regex], [20090805], [mingw-users@sourceforge.net])
AC_CONFIG_SRCDIR([lib/regex.c])
AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])
AM_INIT_AUTOMAKE([1.11 silent-rules dist-xz -Wall -Werror foreign])
AC_CONFIG_HEADERS([config.h])

AC_PROG_CC
gl_EARLY
LT_INIT([win32-dll])


gl_INIT
AC_DEFINE([locale_charset], [libregex_locale_charset],
  [Avoids conflicts with clients of both libregex and gnulib.])

AC_CONFIG_FILES([
	Makefile
	lib/Makefile
	tests/Makefile
])
AC_OUTPUT


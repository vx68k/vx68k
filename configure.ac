# Process this file with autoconf to produce a configure script.
AC_PREREQ([2.69])
AC_INIT([vx68k], [2-alpha.1],
[https://bitbucket.org/kazssym/vx68k/issues/new],,
[https://www.vx68k.org/vx68k])
dnl AC_CONFIG_SRCDIR([])
AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])
AM_INIT_AUTOMAKE([foreign no-define tar-ustar])
# Checks for programs.
AC_PROG_CC
AC_PROG_CXX
# Checks for libraries.
# Checks for header files.
# Checks for typedefs, structures, and compiler characteristics.
# Checks for library functions.
# Checks for other features.
LT_PREREQ([2.4.6])
LT_INIT
PKG_CHECK_MODULES([VM68K], [vm68k])
PKG_CHECK_MODULES([CPPUNIT], [cppunit],, [no_cppunit=yes])
AM_CONDITIONAL([CPPUNIT], [test "$no_cppunit" != yes])
# Configuration actions.
AC_CONFIG_FILES([Makefile])
AC_CONFIG_HEADERS([config.h])
AC_OUTPUT

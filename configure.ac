dnl#                                               -*- Autoconf -*-
dnl# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.61])
AC_INIT([xml2],[0.5.1],[egnor@ofb.net])
AC_CONFIG_AUX_DIR([build-aux])
AM_INIT_AUTOMAKE([1.9.6 -Wall -Werror foreign])
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_SRCDIR([2csv.c])
AC_CONFIG_HEADERS([config.h])dnl

AM_MAINTAINER_MODE

# Checks for programs.
AC_PROG_CC
AC_PROG_EGREP
AC_PROG_LN_S

# Checks for libraries.
PKG_CHECK_MODULES([XML],[libxml-2.0])
AC_SUBST([XML_LIBS])dnl
AC_SUBST([XML_CFLAGS])dnl

# Checks for header files.
AC_CHECK_INCLUDES_DEFAULT
AC_CHECK_HEADERS([stdlib.h string.h unistd.h])dnl

# Checks for typedefs, structures, and compiler characteristics.
AC_C_CONST
AC_TYPE_SIZE_T

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_FUNC_VPRINTF
AC_CHECK_FUNCS([memchr memmove memset strchr strcspn strdup strrchr strstr])dnl

# Output.
AC_CONFIG_FILES([Makefile])
AC_OUTPUT

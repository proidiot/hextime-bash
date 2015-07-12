#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_INIT([hextime-bash], [0.2.3], [charlie@stuphlabs.com])
AC_CONFIG_SRCDIR([src/hextime.pre.in])
AM_INIT_AUTOMAKE([])

# Checks for programs.
AC_CHECK_TOOL([BASH],[bash])
AC_CHECK_TOOL([WGET],[wget])
AC_CHECK_TOOL([AWK],[awk])
AC_CHECK_TOOL([DC],[dc])
AC_CHECK_TOOL([DATE],[date])
AC_CHECK_TOOL([STAT],[stat])

# Checks for libraries.

# Checks for header files.

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.

AC_CONFIG_FILES([Makefile
		 data/Makefile
		 src/Makefile
		 src/hextime.pre
		 test/Makefile])
AC_OUTPUT

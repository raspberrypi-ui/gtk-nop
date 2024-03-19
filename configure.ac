AC_PREREQ([2.71])
AC_CONFIG_MACRO_DIR([m4])
AC_INIT([gtk-nop],[1.0],[http://raspberrypi.com/])
AM_INIT_AUTOMAKE([-Wall foreign subdir-objects no-dist-gzip dist-xz])

#Initialize libtool
LT_PREREQ([2.2])
LT_INIT

# Force to dynamic
AC_DISABLE_STATIC

# Checks for programs.
AC_PROG_CC
AC_PROG_INSTALL
AC_PROG_LN_S
AM_PROG_CC_C_O

# Checks for libraries.
pkg_modules="$pkg_modules gtk+-3.0 >= 3.24.0"
PKG_CHECK_MODULES(PACKAGE, [$pkg_modules])
AC_SUBST(PACKAGE_CFLAGS)
AC_SUBST(PACKAGE_LIBS)

# Checks for typedefs, structures, and compiler characteristics.
AC_C_CONST
AC_C_INLINE

AC_CONFIG_FILES([
    Makefile
    src/Makefile
])
AC_OUTPUT

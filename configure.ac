AC_INIT([imagefs],[0.0])



AM_INIT_AUTOMAKE


AM_CONFIG_HEADER(config.h)

dnl checks for programs.
dnl first check for c/c++ compilers
dnl AC_CHECK_COMPILERS
AC_PROG_CXX

dnl create only shared libtool-libraries
dnl AC_ENABLE_SHARED(yes)

dnl set the following to yes, if you want to create static
dnl libtool-libraries
dnl AC_ENABLE_STATIC(no)

dnl create a working libtool-script
KDE_PROG_LIBTOOL

dnl check for presence of dynamic-loading-library functions
KDE_CHECK_LIBDL

dnl activate the following for some additional tests
dnl   (compat, crypt, socket, nsl, ...)
dnl KDE_MISC_TESTS

dnl add --with-extra-includes and --with-extra-libs switch to ./configure
dnl
dnl AC_REQUIRE([KDE_CHECK_EXTRA_LIBS])
all_libraries="$all_libraries $USER_LDFLAGS"
all_includes="$all_includes $USER_INCLUDES"
AC_SUBST(all_includes)
AC_SUBST(all_libraries)

AC_SUBST(AUTODIRS)

dnl in this space add everything you want to check for
dnl examples are specific headers, libraries, etc.



dnl perform program name transformation
AC_ARG_PROGRAM

dnl add here all your Makefiles. These will be created by configure
AC_OUTPUT(Makefile imagefs/Makefile imagefs/docs/Makefile imagefs/docs/en/Makefile )

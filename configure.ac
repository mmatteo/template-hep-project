# Initialization

AC_INIT([Template Project], [0], [], [template-project])

AC_CONFIG_MACRO_DIR([m4])

AM_INIT_AUTOMAKE([-Wall -Werror])


# Libtool init and language selection

# Workaround for newer vs. older versions of Automake:
m4_ifdef([AM_PROG_AR], [AM_PROG_AR])

AC_LIBTOOL_DLOPEN
AC_PROG_LIBTOOL
AC_PROG_CXX

CXX_PROJECT_INIT
AX_CXX_COMPILE_STDCXX_11([noext])


# Checks for dependencies

ROOTSYS_DEPS([glibs], [-lSpectrum])

CXX_PROJECT_DEPS([])


# Output

AC_CONFIG_HEADERS([config.h])

AC_CONFIG_FILES([
	Makefile
	template-project.pc
	template-project-config
	src/Makefile
	doc/Makefile doc/Doxyfile
])

AC_OUTPUT

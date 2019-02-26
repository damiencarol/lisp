AC_INIT([lisp], [1.0])
AM_INIT_AUTOMAKE([foreign -Wall -Werror])
AC_PROG_CC
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile src/Makefile])

AC_CHECK_FUNCS([memset]) # wanted by: src/mpc.c:127
AC_CHECK_FUNCS([strchr]) # wanted by: src/mpc.c:503
AC_CHECK_FUNCS([strstr]) # wanted by: src/main.c:40
AC_CHECK_FUNCS([strtol]) # wanted by: src/mpc.c:2421
AC_CHECK_HEADERS([stdlib.h]) # wanted by: src/mpc.h:17
AC_CHECK_HEADERS([string.h]) # wanted by: src/mpc.h:20
AC_FUNC_MALLOC # wanted by: src/main.c:11
AC_FUNC_REALLOC # wanted by: src/mpc.c:274
AC_FUNC_STRTOD # wanted by: src/mpc.c:2442
AC_TYPE_SIZE_T # wanted by: src/mpc.h:69

AC_OUTPUT
# Process this file with autoconf to produce a configure script.
AC_INIT(Sato/matchbox/theme.xml)
AM_INIT_AUTOMAKE(matchbox-theme-sato, 0.2)
AM_CONFIG_HEADER(config.h)

# Checks for programs.
AC_PROG_INSTALL

AC_ARG_ENABLE(matchbox-1,
  [  --enable-matchbox-1      Enable Matchbox 1 theme],
  [matchbox1=$enableval], [matchbox1=yes])

AC_ARG_ENABLE(matchbox-2,
  [  --enable-matchbox-2      Enable Matchbox 2 theme],
  [matchbox2=$enableval], [matchbox2=no])

AM_CONDITIONAL(MATCHBOX1, [test "x$matchbox1" = "xyes"])
AM_CONDITIONAL(MATCHBOX2, [test "x$matchbox2" = "xyes"])

AC_OUTPUT([
Makefile
Sato/Makefile
Sato/matchbox/Makefile
Sato/matchbox2/Makefile
])

echo "
           Sato theme for Matchbox Window Manager
           ==========================

        Matchbox WM 1 theme : ${matchbox1}
        Matchbox WM 2 theme : ${matchbox2}
"

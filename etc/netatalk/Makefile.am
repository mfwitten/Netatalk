# Makefile.am for etc/netatlk/

pkgconfdir = @PKGCONFDIR@

sbin_PROGRAMS = netatalk

netatalk_SOURCES = netatalk.c
netatalk_CFLAGS = \
	@EVENT_CFLAGS@ \
	-D_PATH_CONFDIR=\"$(pkgconfdir)/\" \
	-D_PATH_AFPD=\"$(sbindir)/afpd\" \
	-D_PATH_CNID_METAD=\"$(sbindir)/cnid_metad\"

netatalk_LDADD = \
	@EVENT_LIBS@ \
	$(top_builddir)/libatalk/libatalk.la

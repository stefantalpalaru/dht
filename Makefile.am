AM_CFLAGS = @PTHREAD_CFLAGS@

noinst_LTLIBRARIES = libdht.la
libdht_la_SOURCES = dht.c dht.h
libdht_la_DEPENDENCIES = $(builddir)/include/dht

EXTRA_DIST = \
	     CHANGES \
	     CMakeLists.txt \
	     LICENCE \
	     README \
	     dht-example.c \
	     include

BUILT_SOURCES = $(builddir)/include/dht

$(builddir)/include/dht:
	$(MKDIR_P) $(builddir)/include/dht
	cp -a $(srcdir)/dht.h $(builddir)/include/dht/

clean-local:
	-rm -rf $(builddir)/include

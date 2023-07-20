AM_CFLAGS = @PTHREAD_CFLAGS@

noinst_LIBRARIES = libdht.a
libdht_a_SOURCES = dht.c dht.h
libdht_a_DEPENDENCIES = $(builddir)/include/dht
EXTRA_DIST = CHANGES CMakeLists.txt dht-example.c LICENCE README

$(builddir)/include/dht:
	$(MKDIR_P) $(builddir)/include/dht
	cp -a $(srcdir)/dht.h $(builddir)/include/dht/

clean-local:
	-rm -rf $(builddir)/include

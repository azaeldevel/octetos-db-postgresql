AUTOMAKE_OPTIONS=foreign 1.4


lib_LTLIBRARIES = liboctetos-db-postgresql.la


if WITH_ARCHLINUX
DEFINESO = -DARCHLINUX
endif
if WITH_GENTOO
DEFINESO = -DLINUX_GENTOO
endif
if WITH_DEBIAN
DEFINESO = -DLINUX_DEBIAN
endif


liboctetos_db_postgresql_la_CXXFLAGS = $(OCTETOS_DB_ABSTRACT_CFLAGS) $(LIBPQ_CFLAGS) $(DEFINESO)
liboctetos_db_postgresql_la_LIBADD = $(OCTETOS_DB_ABSTRACT_LIBS) $(LIBPQ_CFLAGS)
liboctetos_db_postgresql_la_SOURCES = clientdb-postgresql.cc

octetos_db_includedir = $(includedir)/octetos/db
pkgconfigdir = $(libdir)/pkgconfig
octetos_db_include_HEADERS = clientdb-postgresql.hh
pkgconfig_DATA = octetos-db-postgresql.pc
EXTRA_DIST = octetos-db-postgresql.pc.in
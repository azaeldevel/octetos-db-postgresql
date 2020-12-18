AUTOMAKE_OPTIONS=foreign 1.4


lib_LTLIBRARIES = liboctetos-db-postgresql.la


DEFINITIONS = 
if WITH_MEDIUMWORD
DEFINITIONS += -DOCTETOS_DB_MEDIUMWORD
endif
if WITH_HIGHWORD
DEFINITIONS += -DOCTETOS_DB_HIGHWORD
endif
if WITH_LOWWORD
DEFINITIONS += -DOCTETOS_DB_LOWWORD
endif

if WITH_ARCHLINUX
DEFINITIONS += -DARCHLINUX
endif
if WITH_GENTOO
DEFINITIONS += -DLINUX_GENTOO
endif
if WITH_DEBIAN
DEFINITIONS += -DLINUX_DEBIAN
endif


liboctetos_db_postgresql_la_CXXFLAGS = $(OCTETOS_DB_ABSTRACT_CFLAGS) $(LIBPQ_CFLAGS) $(DEFINITIONS)
liboctetos_db_postgresql_la_LIBADD = $(OCTETOS_DB_ABSTRACT_LIBS) $(LIBPQ_CFLAGS)
liboctetos_db_postgresql_la_SOURCES = clientdb-postgresql.cc

octetos_db_includedir = $(includedir)/octetos/db
pkgconfigdir = $(libdir)/pkgconfig
octetos_db_include_HEADERS = clientdb-postgresql.hh
pkgconfig_DATA = octetos-db-postgresql.pc
EXTRA_DIST = octetos-db-postgresql.pc.in
## Process this file with automake to produce Makefile.in

## Created by Anjuta

AM_CPPFLAGS = \
	-DPACKAGE_LOCALE_DIR=\""$(localedir)"\" \
	-DPACKAGE_SRC_DIR=\""$(srcdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(pkgdatadir)"\" \
	$(OCTETOS_DB_POSTGRESQL_CFLAGS)

AM_CFLAGS =\
	 -Wall\
	 -g

bin_PROGRAMS = octetos_db_postgresql

octetos_db_postgresql_SOURCES = \
	main.cc

octetos_db_postgresql_LDFLAGS = 

octetos_db_postgresql_LDADD = $(OCTETOS_DB_POSTGRESQL_LIBS)



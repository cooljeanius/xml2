ACLOCAL_AMFLAGS = -I m4 --install

AM_CFLAGS = $(XML_CFLAGS)
bin_PROGRAMS = xml2 2xml csv2 2csv
xml2_SOURCES = xml2.c
xml2_LDADD = $(XML_LIBS)
2xml_SOURCES = 2xml.c
2xml_LDADD = $(XML_LIBS)
csv2_SOURCES = csv2.c
2csv_SOURCES = 2csv.c

DISTCLEANFILES = *~ build-aux/*~ autoscan.log

install-exec-hook:
	ln -sf $(DESTDIR)$(bindir)/xml2 $(DESTDIR)$(bindir)/html2
	ln -sf $(DESTDIR)$(bindir)/2xml $(DESTDIR)$(bindir)/2html

distclean-local:
	-rm -rf .deps || rmdir .deps
	-rm -rf autom4te.cache || rmdir autom4te.cache

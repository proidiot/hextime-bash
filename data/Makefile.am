dist_pkgdata_DATA = unix-leap-seconds.list
CLEANFILES = $(dist_pkgdata_DATA)

unix-leap-seconds.list: leap-seconds.list
	cat leap-seconds.list | $(AWK) ' $$1~/^[^#].+/{print $$1-2208988800"\t"$$2}' > unix-leap-seconds.list

install-data-hook:
	touch -t 201501050000.00 $(DESTDIR)$(pkgdatadir)/unix-leap-seconds.list


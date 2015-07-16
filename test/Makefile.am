AUTOMAKE_OPTIONS = dejagnu

check_SCRIPTS = hextime.check
check_DATA = unix-leap-seconds.list
CLEANFILES = $(check_SCRIPTS) $(check_DATA)

hextime.check: $(srcdir)/../src/hextime.pre
	cat $(srcdir)/../src/hextime.pre | $(AWK) '{gsub("@PKGDATADIR@","'$(srcdir)'");print $$0}' > hextime.check
	chmod +x hextime.check

unix-leap-seconds.list: $(srcdir)/../data/leap-seconds.list
	cat $(srcdir)/../data/leap-seconds.list | $(AWK) ' $$1~/^[^#].+/{print $$1-2208988800"\t"$$2}' > unix-leap-seconds.list

DEJATOOL = hextime


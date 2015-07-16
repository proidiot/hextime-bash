dist_bin_SCRIPTS = hextime
CLEANFILES = $(dist_bin_SCRIPTS)

#hextime: hextime.in
#	cat hextime.in | $(AWK) '{gsub("_BASH_","'$(BASH)'");gsub("_AWK_","'$(AWK)'");gsub("_WGET_","'$(WGET)'");gsub("_DC_","$(DC)'");gsub("_DATE_","'$(DATE)'");gsub("_STAT_","'$(STAT)'");gsub("_DATAPATH_","'$(pkgdatadir)'");print $0}' > hextime
#	chmod +x hextime

hextime: $(srcdir)/hextime.pre
	cat $(srcdir)/hextime.pre | $(AWK) '{gsub("@PKGDATADIR@","'$(pkgdatadir)'");print $$0}' > hextime
	chmod +x hextime


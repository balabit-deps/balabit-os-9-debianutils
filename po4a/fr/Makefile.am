AUTOMAKE_OPTIONS=foreign

l = fr
addendum = -a $(top_srcdir)/po4a/$(l)/translator_french.add

TRANSLATE = po4a-translate -f man $(addendum) -p $(top_srcdir)/po4a/po/$(l).po

manlangonedir = $(mandir)/$(l)/man1
dist_manlangone_DATA = which.1

manlangeightdir = $(mandir)/$(l)/man8
dist_manlangeight_DATA = add-shell.8 installkernel.8 remove-shell.8 run-parts.8 savelog.8

%.1: $(top_srcdir)/%.1
	$(TRANSLATE) -m $< -l $@

%.8: $(top_srcdir)/%.8
	$(TRANSLATE) -m $< -l $@

size = 32x32
context = emblems
iconsdir = $(themedir)/$(size)/$(context)
icons_DATA = 				 		\
		emblem-favorite.png 		\
		emblem-important.png 		\
		emblem-noread.png 		\
		emblem-nowrite.png 		\
		emblem-symbolic-link.png 		\
		gnome-netstatus-wireless-idle.png 		\
		gnome-netstatus-wireless-receive.png 		\
		gnome-netstatus-wireless-transmit-receive.png 		\
		gnome-netstatus-wireless-transmit.png 		\
		nwam-connected.png 		\
		nwam-error.png 		\
		nwam-warning.png
EXTRA_DIST = $(icons_DATA)

install-data-local: install-iconsDATA
	(cd $(DESTDIR)$(themedir)/$(size) && $(ICONMAP) -c $(context) -e $(iconsrcdir)/icons/my-mapping.xml)

uninstall-local:
	rm -Rf $(DESTDIR)$(themedir)/$(size)/$(context)

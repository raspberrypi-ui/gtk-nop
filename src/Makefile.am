bin_PROGRAMS = gtk-nop

gtk_nop_CFLAGS = \
	-I$(top_srcdir) \
	-DPACKAGE_LIB_DIR=\""$(libdir)"\" \
	-DPACKAGE_BIN_DIR=\""$(bindir)"\" \
	$(PACKAGE_CFLAGS) \
	$(G_CAST_CHECKS)

gtk_nop_SOURCES = gtk-nop.c

gtk_nop_LDFLAGS = $(DYNAMIC_FLAGS)

gtk_nop_LDADD = \
		$(PACKAGE_LIBS) \
		$(X11_LIBS) \
		$(INTLLIBS)

EXTRA_DIST =

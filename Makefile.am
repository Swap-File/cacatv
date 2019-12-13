plugin_LTLIBRARIES = libgstcacasink.la

libgstcacasink_la_SOURCES = gstcacasink.c gstcacatv.c
libgstcacasink_la_CFLAGS = \
	$(GST_PLUGINS_BASE_CFLAGS) \
	$(GST_BASE_CFLAGS) \
	$(GST_CFLAGS) \
	$(LIBCACA_CFLAGS) \
	-I$(top_srcdir)/gst/videofilter
libgstcacasink_la_LIBADD = \
	$(GST_PLUGINS_BASE_LIBS) \
	-lgstvideo-$(GST_API_VERSION) \
	$(GST_BASE_LIBS) \
	$(GST_LIBS) \
	$(LIBCACA_LIBS) \
	$(LIBM)
libgstcacasink_la_LDFLAGS = $(GST_PLUGIN_LDFLAGS)

noinst_HEADERS = gstcacasink.h gstcacatv.h

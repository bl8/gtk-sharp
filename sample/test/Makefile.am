TARGETS = WidgetViewer.exe 

if ENABLE_LOCAL_CAIRO
local_mono_cairo=$(top_builddir)/cairo/cairo-sharp.dll
else
local_mono_cairo=
endif

assemblies=					\
	$(top_builddir)/glib/glib-sharp.dll	\
	$(top_builddir)/gio/gio-sharp.dll	\
	$(local_mono_cairo)			\
	$(top_builddir)/pango/pango-sharp.dll	\
	$(top_builddir)/atk/atk-sharp.dll	\
	$(top_builddir)/gdk/gdk-sharp.dll	\
	$(top_builddir)/gtk/gtk-sharp.dll

references = $(addprefix -r:, $(assemblies))

noinst_SCRIPTS = $(TARGETS)
CLEANFILES = $(TARGETS)

EXTRA_DIST = $(sources) ChangeLog

sources =			\
	TestCheckButton.cs 	\
	TestColorSelection.cs 	\
	TestComboBox.cs		\
	TestDialog.cs 		\
	TestFlipping.cs 	\
	TestRadioButton.cs 	\
	TestRange.cs 		\
	TestSizeGroup.cs	\
	TestStatusbar.cs 	\
	WidgetViewer.cs

build_sources = $(addprefix $(srcdir)/, $(sources))

WidgetViewer.exe: $(build_sources) $(assemblies)
	$(CSC) $(CSFLAGS) -out:WidgetViewer.exe $(references) $(build_sources)


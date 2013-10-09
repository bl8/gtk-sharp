if ENABLE_LOCAL_CAIRO
local_mono_cairo=$(top_builddir)/cairo/cairo-sharp.dll
else
local_mono_cairo=
endif

pkg = gdk
SYMBOLS = gdk-symbols.xml
INCLUDE_API = $(top_srcdir)/glib/glib-api.xml $(top_srcdir)/cairo/cairo-api.xml $(top_builddir)/gio/gio-api.xml $(top_builddir)/pango/pango-api.xml
METADATA = Gdk.metadata
references = $(top_builddir)/glib/glib-sharp.dll $(top_builddir)/gio/gio-sharp.dll $(top_builddir)/pango/pango-sharp.dll $(local_mono_cairo)
glue_includes = gdk/gdk.h

sources = 			\
	Atom.cs			\
	Color.cs		\
	Device.cs		\
	Display.cs		\
	DisplayManager.cs	\
	EventButton.cs		\
	EventConfigure.cs	\
	EventCrossing.cs	\
	Event.cs		\
	EventDND.cs		\
	EventExpose.cs		\
	EventFocus.cs		\
	EventGrabBroken.cs	\
	EventKey.cs		\
	EventMotion.cs		\
	EventOwnerChange.cs	\
	EventProperty.cs	\
	EventProximity.cs	\
	EventScroll.cs		\
	EventSelection.cs	\
	EventSetting.cs		\
	EventVisibility.cs	\
	EventWindowState.cs	\
	Global.cs		\
	Key.cs			\
	Keymap.cs		\
	Pixbuf.cs		\
	PixbufAnimation.cs	\
	PixbufFrame.cs		\
	PixbufLoader.cs		\
	Pixdata.cs		\
	Point.cs		\
	Property.cs		\
	Rectangle.cs		\
	Screen.cs		\
	Selection.cs		\
	Size.cs			\
	TextProperty.cs		\
	WindowAttr.cs		\
	Window.cs

add_dist = 

include $(top_srcdir)/Makefile.include

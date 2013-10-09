SUBDIRS = . glue

if ENABLE_LOCAL_CAIRO
local_mono_cairo=$(top_builddir)/cairo/cairo-sharp.dll
else
local_mono_cairo=
endif

pkg = pango
METADATA = Pango.metadata
INCLUDE_API = $(top_srcdir)/cairo/cairo-api.xml
SYMBOLS = pango-symbols.xml
references = $(top_builddir)/glib/glib-sharp.dll $(local_mono_cairo)
glue_includes = pango/pango.h

sources =			\
	Analysis.cs		\
	AttrBackground.cs	\
	AttrColor.cs		\
	AttrFallback.cs		\
	AttrFamily.cs		\
	AttrFloat.cs		\
	AttrFontDesc.cs		\
	AttrForeground.cs	\
	AttrGravity.cs		\
	AttrGravityHint.cs	\
	Attribute.cs		\
	AttrInt.cs		\
	AttrIterator.cs		\
	AttrLanguage.cs		\
	AttrLetterSpacing.cs	\
	AttrList.cs		\
	AttrRise.cs		\
	AttrScale.cs		\
	AttrShape.cs		\
	AttrSize.cs		\
	AttrStretch.cs		\
	AttrStrikethrough.cs	\
	AttrStrikethroughColor.cs \
	AttrStyle.cs		\
	AttrUnderline.cs	\
	AttrUnderlineColor.cs	\
	AttrVariant.cs		\
	AttrWeight.cs		\
	Context.cs		\
	Coverage.cs		\
	FontFamily.cs		\
	FontMap.cs		\
	Global.cs		\
	GlyphItem.cs		\
	GlyphString.cs		\
	Item.cs			\
	Layout.cs		\
	LayoutLine.cs		\
	LayoutRun.cs		\
	Matrix.cs		\
	Scale.cs		\
	ScriptIter.cs		\
	TabArray.cs		\
	Units.cs

add_dist =

include $(top_srcdir)/Makefile.include


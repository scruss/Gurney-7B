# Gurney-7B

A minimally-useful tracing of the standard numerals embossed
on credit cards. The geometry should be checked against ISO/IEC 7811---1:2002
should these data be used for official purposes. No claims of
compliance are made here.

As there are only 10 digits in this font, encoding it as a digital
form (TTF, OTF, or otherwise) is left as an exercise for the reader.

## Files

1. *f7b-colour.svg* - an A4 sheet with all 10 digits presented as a
   poster. Each digit is approximately 1284% standard size.

2. *eps folder* - PostScript source files. Each outline is
   approximately 5695% standard size, which is appropriate for a glyph
   in [FontForge](https://fontforge.github.io/ "FontForge").

## Workflow

The rough character outlines were created as short scripts in Python,
using the [Shapely](http://toblerity.org/shapely/project.html
"Shapely") library to handle geometry. A confusing array of support
tools (including, but not limited to: [QCAD](http://www.qcad.org/en/
"QCAD"), [wellknown](https://github.com/mapbox/wellknown "wellknown")
and [OGR](http://www.gdal.org/ "OGR") added the arcs and fillets. The more complex arc
intersections were calculated using
[GeoGebra](http://www.geogebra.org/ "GeoGebra"). Finally, the
outlines --- at this point, mostly in the form of PostScript Level 2
**arct** commands --- were hand-keyed into the EPS files included here.

## Notes on the data

1. There are some typos in the published coordinates, particularly in
   the "1" glyph. Whether these are genuine errors or
   '[trap streets](https://blog.openstreetmap.org/2008/04/01/copyright-easter-eggs/)',
   is hard to tell. The glyphs presented here are intended to be
   visually accurate

2. The published coordinates of the "8" glyph indicate that it is
   only 97.6% as tall as the other digits. This has been carried
   through here.

## Author

Stewart C. Russell - http://scruss.com/blog/

## Thanks

I would like to thank the
[Thai Forest Industry Organization](http://fio.co.th/) for their
generous supply of
[Thai Industrial Standard 1598---2552](http://fio.co.th/p/tisi_fio/fulltext/TIS1598-2552.pdf).


## Licence

WTFPL. (Srsly; see COPYING.)

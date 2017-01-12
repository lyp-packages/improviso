# Improviso: A font package for lilypond

<p align="center">
  <a href="./example.ly">
  <img
    src="https://raw.githubusercontent.com/lyp-packages/improviso/master/example.png">
  </a>
</p>

This package provides the Improviso font for lilypond, created by [Abraham Lee](https://github.com/tisimst), found in  [OpenLilypondFonts](https://github.com/OpenLilypondFonts) and repackaged for usage as a lyp package.

## Installation

Install using [lyp](https://lyp.noteflakes.com):

```bash
$ lyp install improviso
```

## Usage

```lilypond
\require "improviso"

% Use Improviso font and apply associated stylesheet
\useImprovisoStyleSheet

% To use font only:
#(set-global-staff-size 16)  % this MUST go PRIOR to defining the fonts!!!
\paper {
  #(define fonts
    (set-global-fonts
      #:music "improviso"
      #:brace "improviso"
      #:factor (/ staff-height pt 20)
  ))
}
```

Also see the included [example](./example.ly).

## Compatibility with Lilypond versions

This font is known to work in Lilypond version 2.18.2 or later.

FONTLOG for the Improviso font
==============================

This file provides detailed information on the Improviso Font Software. This information should be distributed along with the Improviso fonts and any derivative works.


Basic font information
----------------------

Improviso is a typeface designed by Abraham Lee to resemble the style of traditional hand copyists. This font software is not designed for use in a word-processing application, although all the glyphs may be accessed at their respective Unicode points. It was originally designed for use with GNU LilyPond, the automatic music engraver.

More information about LilyPond can be found at:

http://www.lilypond.org/

Changelog
---------

10 September 2014 (Abraham Lee) Improviso version 1.0
- Initial design to be compatible with LilyPond 2.18.2.

25 October 2014 (Abraham Lee) Improviso version 1.0
- Added WOFF font file support and added piano brace font in OTF, SVG and WOFF formats

20 January 2015 (Abraham Lee) Improviso version 1.0
- Fixed open contour artifacts in some glyphs

23 January 2015 (Abraham Lee) Improviso version 1.0
- Fixed mis-shifted contour in clefs.C_change glyph

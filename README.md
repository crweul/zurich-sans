![Zürich Sans: the name, Aa, and the alphabet with ẞ and ß](images/poster.png)

# Zürich Sans

A sans serif forked from **Inter 4.1** by Rasmus Andersson, set up to stand in for Apple's system font: Inter's
drawings at the system font's size, line height and line length, with:

- a redesigned **ß** and **ẞ**: an arch from the stem that goes over into an s, its stroke one even thickness
  from thin to black
- a long **ſ** with f's crossbar
- a joined **Flemish & Dutch Ĳ ĳ**: J with an I standing on its terminal, and u running into g's tail, with
  i + j joining automatically in Flemish & Dutch text
- **Bulgarian letterforms**: the rounder, handwriting-derived lowercase and the triangular Д and Л that Bulgarian
  readers expect, in roman and italic, automatically in Bulgarian text
- comma accents of one even length (Ș ț ķ ļ ņ ŗ ģ, ď ť ľ)

Every other glyph is Inter's. One variable font in roman and italic, weights
100 to 900 and optical sizes 14 to 32.

## Use

Fonts are in [`fonts/variable`](fonts/variable) (TrueType) and [`fonts/webfonts`](fonts/webfonts) (WOFF2).

```css
@font-face {
  font-family: "Zürich Sans";
  src: url("ZurichSans[opsz,wght].woff2") format("woff2");
  font-weight: 100 900;
  font-style: normal;
}
```

- **Flemish & Dutch:** set `lang="nl-BE"` or `lang="nl"` and typed i + j becomes ĳ, and í j́ becomes ĳ with two
  acutes. Loanwords such as *Beijing*, *Fiji* or *hijab*, and compounds such as *minijurk*, stay as two letters. To
  keep any other word apart, put `&zwnj;` between the i and the j. The Ĳ and ĳ characters (U+0132, U+0133) always
  use the new design.
- **Bulgarian:** set `lang="bg"` and в г д ж з и й ѝ к л п т ц ш щ ю Д Л take their Bulgarian forms. To use them
  without tagging the language, turn on `font-feature-settings: "ss09"`. Russian and every other language
  written in Cyrillic keep the standard forms.
- **Serbian and Macedonian:** their alphabets are all here. Their own letterforms are cursive italic ones (б, г,
  д, п, т), and Zürich's italic is its roman slanted, as Inter's is, so those letters look as they do in other
  languages.

## License

[SIL Open Font License 1.1](LICENSE), with Reserved Font Name "Zürich Sans". The fonts are free to use, including
on websites and in apps. Modified versions must stay under the same license and may not use the name Zürich Sans.

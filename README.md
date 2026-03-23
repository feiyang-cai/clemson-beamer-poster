[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/k4rtik/uchicago-poster)](https://github.com/k4rtik/uchicago-poster/releases)

# Unofficial Poster Template for Clemson University

A fork of [k4rtik/uchicago-poster](https://github.com/k4rtik/uchicago-poster), which is itself a fork of [Gemini](https://github.com/anishathalye/gemini).

Colors follow the [Clemson University Brand Color Guidelines](https://www.clemson.edu/brand/color/).

## Dependencies

* A TeX installation that includes [LuaTeX] or [XeLaTeX]
  * You also need `latexmk` if you want to use the provided `Makefile`
* LaTeX package dependencies including beamerposter (these usually come with
  your TeX installation, but if not, you can get them from [CTAN])
* The following fonts, which must be installed on your system:
  * **[Libre Franklin]** (sans-serif) — free, SIL Open Font License, available on Google Fonts
  * **[Source Serif 4]** (serif) — free, SIL Open Font License, by Adobe, available on Google Fonts

### Installing Fonts

**macOS:** Download the font files from the `fonts/` directory in this repo (or from the links above) and double-click each `.ttf`/`.otf` file to install, or copy them to `~/Library/Fonts/`.

**Linux:** Copy the font files to `~/.local/share/fonts/` and run `fc-cache -f`.

**Windows:** Right-click each font file and select *Install*.

## Usage

1. Clone or download this repository

1. Install the required fonts (see above)

1. In `poster.tex`, set up your paper size, column layout, and scale the
   content as necessary

1. Run `make` to build your poster (requires LuaTeX/XeLaTeX and `latexmk`),
   or compile `poster.tex` directly with your TeX editor using XeLaTeX or LuaLaTeX

## Notes

* The color theme is defined in `beamercolorthemeclemson.sty`. Colors are taken
  directly from the [Clemson brand guidelines](https://www.clemson.edu/brand/color/).
* The layout theme is `beamerthemegemini.sty` (unchanged from upstream).
* **pdfLaTeX is not supported** — use XeLaTeX or LuaLaTeX, as the theme uses `fontspec`.

## FAQ

See the [gemini FAQ] for answers to frequently asked questions.

[LuaTeX]: http://www.luatex.org/
[XeLaTeX]: https://tug.org/xetex/
[CTAN]: https://ctan.org/
[Libre Franklin]: https://fonts.google.com/specimen/Libre+Franklin
[Source Serif 4]: https://fonts.google.com/specimen/Source+Serif+4
[gemini FAQ]: https://github.com/anishathalye/gemini/wiki/FAQ

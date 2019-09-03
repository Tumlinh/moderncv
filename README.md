#moderncv: a modern curriculum vitae class#

**Moderncv** provides a documentclass for typesetting curricula vitae in various styles. Moderncv aims to be both straightforward to use and customizable, providing five ready-made styles (classic, casual, banking, oldstyle and fancy) and allowing one to define his own by modifying colors, fonts, icons, etc.  
Most commands are defined in such a way that arguments are optional.  
Until a decent manual is written, one can always look in the "examples" directory for some examples. Documents can be compiled into dvi, ps or pdf.


This is a fork of [that repository](https://github.com/xdanaux/moderncv).

---

### Yet another moderncv fork. Why?
The main [repo](https://github.com/xdanaux/moderncv) has not been updated since 2016.

A good reason to use this fork is to be able to use a plentifulness of new icons through [FontAwesome 5](https://fontawesome.com).  
FontAwesome offers more than 7000 icons. The gallery can be found [here](https://fontawesome.com/icons?d=gallery).  
Font icons have several properties that images do not have, inherited from their textual nature:
+ they are scalable
+ they are incredibly easy to use (one single command)
+ they can be selected, copied, pasted
+ they are coloured according to the font colour

---

### How to
+ Install [`texlive-latex-extra`](https://tug.org/texlive/), which contains many LaTeX packages including [`fontawesome5`](https://www.ctan.org/pkg/fontawesome5)
+ Clone this repo
+ Start a new TeX document inside the repo
+ Compile it using your favourite TeX engine. So far, `moderncv` can be compiled with `pdfTeX`, `XeTeX` and `LuaTeX` (give or take some warnings)
  ```
  latexmk -pdf template.tex
  ```
  or
  ```
  latexmk -xelatex template.tex
  ```
  or
  ```
  latexmk -lualatex template.tex
  ```

Depending on [`fontawesome5`](https://www.ctan.org/pkg/fontawesome5) and your FontAwesome version (free or professional), every icon may not be available. A list of supported icons along with their associated TeX command can be found in the `fontawesome5-mapping.def` file.
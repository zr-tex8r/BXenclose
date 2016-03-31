BXenclose Package
=================

LaTeX: To enclose the document body with some pieces of code

Blah....

### System requirement

  * TeX format: LaTeX.
  * TeX engine: Anything.
  * Dependent packages: None.

### Installation

  - `*.sty` → $TEXMF/tex/latex/BXenclose

### License

This package is distributed under the MIT License.

The bxenclose Package
---------------------

### Package Loading

    \usepackage{bxenclose}

No options are available.

### Usage

    \enclosebodywith{<begin>}{<end>}

Makes the document body enclosed with `<begin>`  and `<end>`.
That is, `<begin>` is executed immediately before the body text
(probably after other “begin-document hooks” provided by LaTeX itself
and other packages) and `<end>`  is executed immediately after the
the body text (probably before other “end-document hooks”).
Note that `<begin>` code does not belong to the preamble.

Revision History
----------------

  * Version 0.2  ‹2016/04/01›
      - The first public version.

--------------------
Takayuki YATO (aka. "ZR")  
http://zrbabbler.sp.land.to/

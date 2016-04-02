BXenclose Package
=================

LaTeX: To enclose the document body with some pieces of code
                                                            
The package enables authors to designate in the preamble to make the
document body enclosed with the given pieces of code. As is known,
there are already various mechanisms provided by LaTeX kernel or
packages that attach “hooks” at the beginning and end of documents.
This package tries harder to win the race, that is, place the given
code as close to the real document body as possible.

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

This package defines the following single command:

    \enclosebodywith{<begin>}{<end>}

This command makes the document body enclosed with `<begin>`  and
`<end>`. That is, `<begin>` is executed immediately before the body
text (probably after other “begin-document hooks” provided by LaTeX
itself and other packages) and `<end>`  is executed immediately after
the body text (probably before other “end-document hooks”).

Note that both `<begin>` and `<end>` code are treated as part of the
document body. In particular, `<begin>` code cannot contain any
preamble-restricted commands (such as `\listfiles`).

Revision History
----------------

  * Version 0.2  〈2016/04/01〉
      - The first public version.

--------------------
Takayuki YATO (aka. "ZR")  
http://zrbabbler.sp.land.to/

# cv
My personal curriculum vitae. Get the latest [pdf version](https://github.com/geeanlooca/cv/releases/latest/download/cv.pdf) or [Word format](https://github.com/geeanlooca/cv/releases/latest/download/cv.docx).

## How to set up the repository
Just clone the repository and the submodules:
```
git clone --recurse-submodules git://github.com/geeanlooca/cv.git
```

## How to generate the pdf
A LaTeX distribution providing `pdflatex` is needed, along with `biblatex` and `biber`.
Issue the following command

```
pdftex main.tex
biber main
pdftex main.tex
pdftex main.tex
```

## How to generate the Word document
This requires `pandoc` (only tested on versions `3.1.1` and `3.1.3`). 
```
pandoc -s main.tex --bibliography .\bib\bibliography.bib --csl=ieee.csl --citeproc  -o cv.docx
```
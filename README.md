# cv
My personal curriculum vitae. Get the lasted version [here](https://github.com/geeanlooca/cv/releases/latest/download/cv.pdf) .

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
# tex-novamath

"Nova Mathematica" symbola et macrones LaTeX in Latina

"Nova Mathematica" LaTeX symbols and macros in Latin.

## Usage

It might be worthy to read this [tex.stackexchange](https://tex.stackexchange.com/questions/1137/where-do-i-place-my-own-sty-or-cls-files-to-make-them-available-to-all-my-te)
question.

Use
```bash
kpsewhich -var-value=TEXMFHOME
```
to find the install directory of TeX packages. This directory will be referred
to as `$TEXMFHOME`.

Then, create the directory `$TEXMFHOME/tex/latex/local` and clone
`tex-novamath` into it.

Then execute
```bash
texhash $TEXMFHOME
```
to update the available tex packages.

The following packages are available:

1. novamath-symbola: Redefined Latinised mathematics symbols
2. novamath-thm: Theorem environments (theorema, propositio, etc.) The option
	[lingua=...] can be fed into the package to select the language. Currently
	latina and english are supported.
3. novamath-physica: Physical symbols
4. novamath: Latin NovaMathematica preamble.

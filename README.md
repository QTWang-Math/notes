# Notes

Personal notes on representation theory, geometric representation theory, and related topics in algebraic geometry. It is still evolving, and notation or exposition may change over time.

[Read the latest PDF](temp/main.pdf)

> The bad news is that we have still a long way to go.<br>
> The good news is that we have still a long way to go.
>
> - Alain Fournier, 1998


These notes are organized chronologically. They contain definitions, examples, calculations, references, and working observations rather than a finished exposition.

## Build

Compile the complete notes with XeLaTeX:

```bash
latexmk -xelatex -outdir=temp main.tex
```

The generated PDF is available at `temp/main.pdf`.

For a faster local build containing only the active year, run:

```bash
latexmk -xelatex -outdir=temp current.tex
```

When editing `chapters/2026.tex`, LaTeX Workshop uses this faster entry point automatically. GitHub Actions always builds the complete document and keeps `temp/main.pdf` up to date.

## Author

Qiutong Wang

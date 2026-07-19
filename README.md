# Notes

Personal notes on representation theory, geometric representation theory, and related topics in algebraic geometry.

The material is organized chronologically and records definitions, examples, calculations, references, and working observations collected while studying. These are evolving research notes rather than a finished textbook, so notation and exposition may change over time.

## Topics

The notes currently cover themes including:

- algebraic groups, tori, root data, and pinnings;
- Harish-Chandra modules and Casselman-Wallach representations;
- coherent continuation and regular characters;
- nilpotent orbits, wavefront sets, and Whittaker models;
- the orbit method and geometric quantization;
- flag varieties, conormal bundles, and characteristic cycles;
- perverse sheaves, local systems, and D-modules;
- symplectic singularities, Poisson geometry, and quantization.

## Repository Structure

```text
.
|-- main.tex            Main document, macros, and theorem environments
|-- chapters/
|   |-- 2023.tex        Notes written in 2023
|   |-- 2024.tex        Notes written in 2024
|   |-- 2025.tex        Notes written in 2025
|   `-- 2026.tex        Notes written in 2026
|-- references.bib      Bibliography database
|-- TooYoung.sty        Custom Young diagram/tableau utilities
`-- temp/               LaTeX build output
```

The active year is selected in `main.tex` with `\includeonly`. Remove that line, or list additional chapters there, to build more than one year at a time.

## Building

A TeX distribution with XeLaTeX, Biber, and the packages imported by `main.tex` is required. With `latexmk` installed, run:

```bash
latexmk -xelatex -outdir=temp main.tex
```

The generated document will be available at `temp/main.pdf`. Bibliography processing is configured through `biblatex` with the Biber backend and is handled automatically by `latexmk`.

To remove generated files:

```bash
latexmk -C -outdir=temp main.tex
```

## Conventions

- Theorem-like environments and most notation macros are defined in `main.tex`.
- Bibliographic entries belong in `references.bib`.
- New notes should be added to the chapter corresponding to the current year.
- `TooYoung.sty` provides project-specific commands for Young diagrams and tableaux.

## Status

This repository is maintained as a personal, continuously updated notebook. Statements may be incomplete, provisional, or recorded without full proofs. Corrections and clarifications are added as the material develops.

## Author

Wang Qiutong

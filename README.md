# PythonLecture

Introductory Python lecture slides for beginners, written as a LaTeX Beamer
presentation.

The repository includes both the source deck (`python.tex`) and a generated PDF
(`python.pdf`).

## Lecture Contents

The current deck covers:

- The 2026 class Python setup and script-based workflow
- What Python is and how interpreted languages differ from compiled languages
- Basic input and output with `print()` and `input()`
- Core data types and operators:
  - integers
  - floating-point numbers
  - strings
  - booleans and comparisons
  - arithmetic operators
  - lists
  - indexing
  - slicing
- File I/O with `with open(...)`
- Control flow with `if`, `for`, and `while`
- Functions, exception handling, and modules

## Files

| Path | Description |
| --- | --- |
| `.python-version` | Python version pin for the 2026 class examples. |
| `python.tex` | Main LaTeX Beamer source file for the lecture slides. |
| `python.pdf` | Generated slide deck. |
| `figures/python.png` | Python logo used in the introduction. |
| `figures/run1.png` | Screenshot/example for running Python in an interpreter. |
| `figures/run2.png` | Screenshot/example for running a Python script. |
| `LICENSE` | Project license. |

## Requirements

The classroom examples assume Python 3.14.5. The repository includes
`.python-version` so pyenv-compatible setups can select that version for the
project.

To rebuild the PDF, install a LaTeX distribution that includes Beamer. On macOS,
MacTeX provides the required tools.

Useful commands:

```sh
latexmk -pdf python.tex
```

If `latexmk` is not available, run `pdflatex` twice so the table of contents and
references are resolved:

```sh
pdflatex python.tex
pdflatex python.tex
```

To remove LaTeX auxiliary files after building:

```sh
latexmk -c python.tex
```

## Editing the Slides

Update `python.tex` for slide text and structure. Place any additional images in
`figures/`, then reference them from the LaTeX source with `\includegraphics`.

After editing, rebuild `python.pdf` and review the generated slides before
sharing them.

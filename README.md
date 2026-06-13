# PythonLecture

Introductory Python lecture slides for beginners, written as a LaTeX Beamer
presentation.

The repository includes both the source deck (`python.tex`) and a generated PDF
(`python.pdf`).

## Lecture Contents

The current deck covers:

- What Python is and how interpreted languages differ from compiled languages
- Running Python through an interpreter or as a script
- Basic input and output with `print()` and `input()`
- Core data types and operators:
  - integers
  - floating-point numbers
  - arithmetic operators
  - lists
  - indexing

The source also contains section placeholders for advanced I/O, control flow,
functions, exception handling, and modules.

## Files

| Path | Description |
| --- | --- |
| `python.tex` | Main LaTeX Beamer source file for the lecture slides. |
| `python.pdf` | Generated slide deck. |
| `figures/python.png` | Python logo used in the introduction. |
| `figures/run1.png` | Screenshot/example for running Python in an interpreter. |
| `figures/run2.png` | Screenshot/example for running a Python script. |
| `LICENSE` | Project license. |

## Requirements

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

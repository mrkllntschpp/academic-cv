# Academic CV — Mark Tschopp, PhD

The LaTeX source for my academic CV — and a reusable template, if you'd like to build your own.

📄 **[Download the compiled PDF](tschopp-cv.pdf)** &nbsp;·&nbsp; 🌐 **[marktschopp.github.io](https://marktschopp.github.io)**

## Why this is public

People occasionally ask how I format my CV, so here's the full source. It's built on the classic `res` LaTeX class with a modular structure I've refined over the years — one file per section, assembled by a short main document. Borrow the format, the section layout, or the whole thing as a starting point for your own.

## Building it

Requires a LaTeX distribution (TeX Live, MiKTeX, MacTeX). From the project root:

```bash
pdflatex tschopp-cv.tex
pdflatex tschopp-cv.tex   # second pass resolves cross-references
```

Output: `tschopp-cv.pdf`.

## Structure

| File | What it is |
|---|---|
| `tschopp-cv.tex` | Main document — preamble, contact block, and the section includes |
| `res.cls`, `res.sty` | The résumé document class and styling |
| `src/01-education.tex` … `src/16-service.tex` | One file per CV section, included in order |

Tailoring the CV for a specific purpose is as simple as commenting or uncommenting `\include{}` lines in the main file — each section is self-contained, so you can reorder or drop sections without touching the rest.

## A note on reuse

The formatting and structure are free to reuse under the [MIT License](LICENSE). The *content* — my education, publications, and so on — is mine; swap in your own.

Built on the `res` document class by Michael DeCorte, with customizations of my own.

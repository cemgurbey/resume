# resume

LaTeX source for my résumé: [`resume.tex`](resume.tex).

The compiled PDF is [`resume.pdf`](resume.pdf) — viewable right in the browser on GitHub.

## How the PDF stays up to date

A GitHub Actions workflow (`.github/workflows/build-pdf.yml`) runs on every push to `main` that touches `resume.tex`:

1. Compiles `resume.tex` with TeXLive (`latexmk -pdf`) via `xu-cheng/latex-action`, installing the font packages the template needs (Montserrat, Lato, Nunito, FontAwesome5, …).
2. The `github-actions` bot commits the rebuilt `resume.pdf` back to the repo.

The workflow only triggers on changes to `resume.tex` (or itself), so the bot's PDF-only commit doesn't re-trigger it.

## Build locally

```sh
latexmk -pdf resume.tex
```

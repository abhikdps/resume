# Resume

A LaTeX-based resume. The compiled PDF is automatically regenerated on every push via GitHub Actions.

## Structure

```text
resume.tex              # Main entry point
custom-commands.tex # Shared LaTeX macros
src/
  heading.tex
  education.tex
  experience.tex
  projects.tex
  skills.tex
```

## Build locally

Requires a LaTeX distribution (`pdflatex`). On Ubuntu/Debian:

```bash
sudo apt-get install -y \
  texlive-latex-extra \
  texlive-fonts-extra \
  texlive-fonts-recommended \
  texlive-lang-english

pdflatex resume.tex
mv resume.pdf Abhinav-Anand.pdf
```

The compiled `Abhinav-Anand.pdf` is committed to this repo and kept up to date by CI.

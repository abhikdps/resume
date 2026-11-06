# Resume

A one-page, text-based, single-column LaTeX resume for backend, platform engineering, and developer tools roles.

## Structure

- `resume.tex`: document layout and section order
- `custom-commands.tex`: shared formatting macros
- `src/`: contact details, summary, experience, projects, skills, and education
- `Abhinav-Anand.pdf`: compiled resume

## Build locally

Using a LaTeX distribution with pdfLaTeX:

```sh
pdflatex -interaction=nonstopmode -halt-on-error -jobname=Abhinav-Anand resume.tex
```

Or using Tectonic:

```sh
tectonic resume.tex
mv resume.pdf Abhinav-Anand.pdf
```

## Content and review

Keep performance measurements tied to documented workloads and environments. Add professional impact numbers only when supported by records or a defensible reconstruction. Match relevant terminology to a specific job description without adding skills or experience you do not have.

The layout uses standard headings, visible contact links, selectable text, and no tables or icon fonts. Check PDF text extraction and visual layout after edits. No universal ATS score is implied.

The existing GitHub Actions workflow regenerates and commits the PDF after pushes to `main`. Local compilation does not push or commit changes.

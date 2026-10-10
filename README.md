# English CV - LaTeX

A clean, ATS-friendly, one-page CV template intended for local editing and Overleaf.

## Edit

Open `main.tex` and replace every placeholder, especially:

- name and contact details;
- profile summary;
- education and dates;
- experience and quantified achievements;
- projects, technical skills, and activities.

Keep bullet points concise and begin each one with a strong action verb. Whenever possible,
include a measurable result.

## Compile locally

With a TeX distribution installed:

```bash
latexmk -pdf main.tex
```

Clean generated files with:

```bash
latexmk -c
```

## Use with Overleaf

Import the GitHub repository into Overleaf and set `main.tex` as the main document. The
template uses pdfLaTeX and only standard TeX Live packages.

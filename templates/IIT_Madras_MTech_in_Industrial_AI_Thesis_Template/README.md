# IIT Madras MTech in Industrial AI Thesis Template

This folder contains the extracted LaTeX thesis template for the IIT Madras Master of Technology (MTech) in Industrial Artificial Intelligence program.

## Main Template File

The main entry point for this template is:

- **`thesis.tex`** – The primary LaTeX document that compiles the entire thesis

## Template Class and Style Files

- `iitmdissertation.cls` – The main document class for the dissertation
- `iitmdissertation.sty` – Supplementary style file with additional formatting
- `iitm.bst` – BibTeX style file for references

## Folder Structure

```
.
├── thesis.tex                    # Main LaTeX entry point
├── iitmdissertation.cls          # Document class
├── iitmdissertation.sty          # Style definitions
├── iitm.bst                      # Bibliography style
├── references.bib                # Bibliography database
├── 0-prematter/                  # Preliminary pages (certificates, dedication, quote)
│   ├── pre-cert-attr.tex
│   ├── pre-cert-guides.tex
│   ├── pre-dedication.tex
│   ├── pre-list-of-publications.tex
│   └── pre-quote.tex
├── 1-frontmatter/                # Front matter (abstract, acknowledgements, notation)
│   ├── front-abstract.tex
│   ├── front-acknowledgements.tex
│   ├── front-glossary-abbreviations.tex
│   └── front-notation.tex
├── 2-mainmatter/                 # Main chapters and appendices
│   ├── chapters/
│   │   ├── chap-introduction.tex
│   │   ├── chap-lists.tex
│   │   ├── chap-maths.tex
│   │   └── chap-figures-tables.tex
│   └── appendices/
│       └── appn-general-notes.tex
├── 3-backmatter/                 # Back matter (committee, CV)
│   ├── back-committee.tex
│   └── back-cv-education.tex
├── images/                       # Image assets
│   ├── iitm-logo.png
│   └── (various sample images)
└── zz-imp/                       # Implementation templates
    ├── back-imp-cv.tex
    ├── pre-imp-cert.tex
    ├── pre-imp-cover.tex
    └── pre-imp-do-covers.tex
```

## Building the Document

This is a LaTeX template. To compile, use either:

### Option 1: pdflatex + bibtex

```bash
pdflatex thesis.tex
bibtex thesis
pdflatex thesis.tex
pdflatex thesis.tex
```

### Option 2: latexmk (recommended)

```bash
latexmk -pdf thesis.tex
```

### Option 3: xelatex (for Unicode/fonts support)

```bash
xelatex thesis.tex
bibtex thesis
xelatex thesis.tex
xelatex thesis.tex
```

## Configuration

Edit `thesis.tex` to customize:
- `\dissertationDepartment{...}` – Your department name
- `\dissertationAuthorName{...}` – Your name
- `\dissertationTitle{...}` – Your thesis title
- `\dissertationMonth{...}` and `\dissertationYear{...}` – Submission date
- `\dissertationGuides{...}` – Your thesis advisor(s)

## Notes

- The template uses `mtech` option for MTech degrees (can also be used with `phd`, `ms`, `btech`)
- A `tutorial.pdf` was included in the original archive but has been excluded as a build artifact
- Edit the `.tex` files in the numbered folders to add your content

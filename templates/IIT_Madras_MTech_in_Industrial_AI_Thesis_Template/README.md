# IIT Madras MTech in Industrial AI Thesis Template

This folder contains the extracted LaTeX thesis/dissertation template from `IIT Madras MTech in Industrial AI Thesis Template.zip`.

## Main Template File

The main entry point for this template is:
- **`thesis.tex`** - Main LaTeX document file

## Template Files

The template uses the following custom class and style files:
- **`iitmdissertation.cls`** - Document class for IIT Madras dissertations (supports PhD, MS, MTech, BTech)
- **`iitmdissertation.sty`** - Supporting style file
- **`iitm.bst`** - Bibliography style file for BibTeX

## Directory Structure

```
IIT_Madras_MTech_in_Industrial_AI_Thesis_Template/
├── thesis.tex                  # Main document (edit this)
├── iitmdissertation.cls        # Document class
├── iitmdissertation.sty        # Style file
├── iitm.bst                    # Bibliography style
├── references.bib              # Bibliography database
├── 0-prematter/                # Preliminary matter (quotes, dedication, certificates)
│   ├── pre-cert-attr.tex
│   ├── pre-cert-guides.tex
│   ├── pre-dedication.tex
│   ├── pre-list-of-publications.tex
│   └── pre-quote.tex
├── 1-frontmatter/              # Front matter (abstract, acknowledgements, glossary)
│   ├── front-abstract.tex
│   ├── front-acknowledgements.tex
│   ├── front-glossary-abbreviations.tex
│   └── front-notation.tex
├── 2-mainmatter/               # Main content (chapters and appendices)
│   ├── appendices/
│   │   └── appn-general-notes.tex
│   └── chapters/
│       ├── chap-figures-tables.tex
│       ├── chap-introduction.tex
│       ├── chap-lists.tex
│       └── chap-maths.tex
├── 3-backmatter/               # Back matter (committee, CV)
│   ├── back-committee.tex
│   └── back-cv-education.tex
├── images/                     # Image assets
│   ├── iitm-logo.png
│   └── [sample images]
└── zz-imp/                     # Implementation files for covers/certificates
    ├── back-imp-cv.tex
    ├── pre-imp-cert.tex
    ├── pre-imp-cover.tex
    └── pre-imp-do-covers.tex
```

## Build Instructions

This is a LaTeX template that requires a TeX distribution (e.g., TeX Live, MiKTeX).

### Recommended Build Sequence

```bash
# Option 1: Using pdflatex and bibtex
pdflatex thesis.tex
bibtex thesis
pdflatex thesis.tex
pdflatex thesis.tex

# Option 2: Using latexmk (recommended for automation)
latexmk -pdf thesis.tex

# Option 3: Using xelatex (if using custom fonts)
xelatex thesis.tex
bibtex thesis
xelatex thesis.tex
xelatex thesis.tex
```

### Dependencies

- LaTeX2e with standard packages
- BibTeX for bibliography processing
- The `multirow` package (included in most TeX distributions)

## Usage

1. Edit `thesis.tex` to update your personal information (name, department, title, etc.)
2. Add your content to the chapter files in `2-mainmatter/chapters/`
3. Add your bibliography entries to `references.bib`
4. Compile using the build instructions above

## Files Omitted

The following files were excluded during extraction:
- `tutorial.pdf` - Build artifact (PDF documentation)

## Notes

- The original zip file remains at the repository root
- This template supports multiple degree types via class options: `phd`, `ms`, `mtech`, `btech`

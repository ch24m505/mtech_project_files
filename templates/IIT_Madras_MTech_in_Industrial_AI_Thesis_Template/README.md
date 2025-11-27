# IIT Madras MTech in Industrial AI Thesis Template

This directory contains the extracted LaTeX thesis template for IIT Madras MTech in Industrial AI program.

## Contents

### Main Template Files

| File | Description |
|------|-------------|
| `thesis.tex` | **Main entry point** - The primary LaTeX file to compile |
| `iitmdissertation.cls` | Document class file defining thesis structure and styling |
| `iitmdissertation.sty` | Style file with additional formatting and package requirements |
| `iitm.bst` | Bibliography style file for citations |
| `references.bib` | Sample bibliography database |

### Directory Structure

```
.
├── 0-prematter/          # Preliminary pages (dedication, certificate, etc.)
├── 1-frontmatter/        # Front matter (abstract, acknowledgements, glossary)
├── 2-mainmatter/         # Main content
│   ├── appendices/       # Appendix files
│   └── chapters/         # Chapter files
├── 3-backmatter/         # Back matter (committee, CV)
├── images/               # Sample images and IIT Madras logo
└── zz-imp/               # Implementation files for covers and certificates
```

### Top-Level Files and Directories

- `thesis.tex` - Main LaTeX entry point
- `iitmdissertation.cls` - Document class
- `iitmdissertation.sty` - Style package
- `iitm.bst` - Bibliography style
- `references.bib` - Bibliography database
- `0-prematter/` - Preliminary matter templates
- `1-frontmatter/` - Front matter templates
- `2-mainmatter/` - Main content templates
- `3-backmatter/` - Back matter templates
- `images/` - Images including IIT Madras logo
- `zz-imp/` - Implementation files

## Building the Thesis

This template uses standard LaTeX with BibTeX for bibliography management.

### Prerequisites

- A LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- The following LaTeX packages are required (included in most distributions):
  - microtype, setspace, graphicx, subcaption
  - mathtools, booktabs, array, amsthm, amssymb
  - enumitem, natbib, eso-pic, glossaries

### Compilation Commands

To build the thesis, run the following commands in order:

```bash
# Using pdflatex
pdflatex thesis.tex
bibtex thesis
pdflatex thesis.tex
pdflatex thesis.tex
```

Or using latexmk (recommended for automated builds):

```bash
latexmk -pdf thesis.tex
```

### Output

The compilation will generate `thesis.pdf` containing your formatted thesis.

## Usage Notes

1. Edit `thesis.tex` to customize:
   - Department name
   - Author name and date of birth
   - Thesis title
   - Guide/supervisor name
   - Submission date

2. The template supports different degree types via options:
   - `mtech` - Master of Technology (default for this template)
   - `phd` - Doctor of Philosophy
   - `ms` - Master of Science
   - `btech` - Bachelor of Technology

3. Add your chapters in the `2-mainmatter/chapters/` directory

4. Update `references.bib` with your bibliography entries

## Files Excluded

The following files were excluded from this extraction:
- `tutorial.pdf` - Tutorial document (build artifact)

## Original Source

This template was extracted from: `IIT Madras MTech in Industrial AI Thesis Template.zip`

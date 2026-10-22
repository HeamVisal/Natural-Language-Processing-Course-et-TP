# Repository Guidelines

## Project Structure & Module Organization

This workspace groups coursework in `ADVProgrm/` (advanced programming), `NLP/`,
`TSA/` (time series), `WR/` (information retrieval), and `1English/`.
`ADVProgrm/`, `TSA/`, and `WR/` have independent Git histories; run Git commands
inside the relevant directory or use `git -C WR ...`.

Store references in `Course/`, practical work in `TP1/`, `TP2/`, etc., and English
activities in `1English/ClassActivity/`. Keep editable sources, notebooks, and
submission exports together within each assignment.

## Build, Test, and Development Commands

There is no workspace-wide build or dependency manifest. Install tools and
dependencies for the assignment being edited. Run these commands from this directory:

- `jupyter lab WR/TP2/TP2_Text_Processing_BoW_Ngram.ipynb`: open the Python notebook.
- `quarto preview TSA/TP1/Week1/TSAW1.qmd`: preview the R exercise with live updates.
- `quarto render TSA/TP1/Week1/TSAW1.qmd`: generate its HTML output.

The WR notebook uses NLTK, pandas, Transformers, and scikit-learn, with downloads
for language resources and model files. The Quarto exercise requires R and the
`TSA` package.

## Coding Style & Naming Conventions

Follow the PEP 8 guidance in `ADVProgrm/TP1/README.md`: four-space indentation,
`snake_case` functions and variables, `PascalCase` classes, and `UPPER_CASE`
constants. Ruff is documented there; run `ruff check .` and
`ruff format --check .` within the relevant course directory when applicable.
No shared formatter configuration is checked in.

Preserve assignment numbering and required submission filenames, such as
`TP1_e20221349_HEAMVisal.pdf`. Keep Markdown headings descriptive and links relative.

## Testing Guidelines

No automated test suite, testing framework, or coverage threshold is configured.
Run completed notebook exercises from a fresh kernel and document expected failures
from unfinished TODO cells. Render changed Quarto documents. Open modified PDFs,
DOCX files, and HTML pages to check layout, formulas, and navigation. Record the
checks performed when submitting changes.

## Commit & Pull Request Guidelines

Existing commits use short descriptions such as `Add TP1 class summary` and
`Ch3 docs added`; no uniform prefix scheme is established. Prefer an imperative
summary naming the course or assignment. Keep commits focused.

Follow `ADVProgrm/README.md`: use a separate branch and dedicated folder per
activity, merging activity work when the subject ends. For pull requests, describe
the assignment, changed files, and validation; link an issue when applicable and
attach screenshots for visual changes.

## Course Material Handling

Preserve instructor originals. Respect the private-study restriction for copied
NLP lectures described in `NLP/AppsScptCopy.txt`.

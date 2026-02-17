# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LaTeX-based CV/Resume project using the **Awesome CV** template, structured to comply with the TENK 2020 (Finnish National Board on Research Integrity) guidelines for academic researchers.

## Build Commands

Requires a full TeX distribution (e.g., TeX Live) with **XeLaTeX** (needed for TTF font support and Unicode):

```bash
xelatex cv.tex           # Compile the full CV
xelatex resume.tex       # Compile the résumé
xelatex coverletter.tex  # Compile the cover letter
```

Each produces a corresponding PDF in the project root.

## Architecture

- **`awesome-cv.cls`** — Core LaTeX class file defining all styling, custom commands, and layout. This is the template engine shared by all documents.
- **`cv.tex`** — Monolithic CV document; all content is inline in one file.
- **`resume.tex`** — Modular résumé; includes section files from `resume/` via `\input{}`.
- **`coverletter.tex`** — Cover letter template.
- **`resume/`** — Individual `.tex` section files (degrees, experience, awards, etc.). Several are placeholders (funding, supervision, teaching, merits, impact) marked with TODO comments.
- **`cv/`** — Section files for the CV (education, experience, honors, skills, etc.), though `cv.tex` currently embeds its content directly.
- **`fonts/`** — Roboto font family (11 variants) and FontAwesome TTF, loaded by `awesome-cv.cls` via `fontspec`.

## Key Conventions

- Color theme is set per document (e.g., `\colorlet{awesome}{awesome-skyblue}` in cv.tex, `awesome-red` in coverletter.tex).
- Personal info is configured via commands like `\name`, `\position`, `\email`, `\github`, `\linkedin` in each main `.tex` file's preamble.
- The resume uses `\input{resume/<section>.tex}` for modularity — add new sections by creating a file in `resume/` and adding the corresponding `\input` in `resume.tex`.
- The `orcidlink` package is used in `cv.tex` for ORCID integration.

# Personal CV and Resume

This repository contains my personal Curriculum Vitae (CV) and Résumé, built using a modified version of the "Awesome CV" LaTeX template. Both documents are structured to align with the recommendations of the Finnish National Board on Research Integrity TENK 2020 template for researchers.

## Documents

*   **`cv.tex`**: My comprehensive Curriculum Vitae, following the TENK guidelines.
*   **`resume.tex`**: My concise Résumé, also structured according to TENK recommendations. This document utilizes a modular approach, drawing content from individual `.tex` files within the `resume/` directory.
*   **`coverletter.tex`**: A LaTeX template for a cover letter.

## How to Use

To compile these documents, you will need a full TeX distribution installed on your system (e.g., TeX Live).

Navigate to the root directory of this repository in your terminal and execute the following commands to generate the PDF files:

*   **To compile the CV:**
    ```bash
    xelatex cv.tex
    ```

*   **To compile the Résumé:**
    ```bash
    xelatex resume.tex
    ```

*   **To compile the Cover Letter:**
    ```bash
    xelatex coverletter.tex
    ```

Each command will generate a corresponding PDF file (e.g., `cv.pdf`, `resume.pdf`, `coverletter.pdf`) in the same directory.

## Structure

The project structure is organized as follows:

*   `awesome-cv.cls`: The core LaTeX class file for the template.
*   `cv.tex`: Main CV document.
*   `resume.tex`: Main Résumé document, which includes sections from the `resume/` directory.
*   `coverletter.tex`: Main Cover Letter document.
*   `fonts/`: Directory containing custom fonts used in the documents.
*   `cv/`: Contains modular `.tex` files for different sections of the CV (if applicable, similar to `resume/`).
*   `resume/`: Contains modular `.tex` files for different sections of the Résumé, including:
    *   `degrees.tex`
    *   `other_education.tex`
    *   `language_skills.tex`
    *   `current_employment.tex`
    *   `previous_experience.tex`
    *   `funding.tex` (placeholder)
    *   `output.tex`
    *   `supervision.tex` (placeholder)
    *   `teaching.tex` (placeholder)
    *   `awards.tex`
    *   `merits.tex` (placeholder)
    *   `impact.tex` (placeholder)

## TENK CV Template Compliance

The CV and Résumé are structured to adhere to the sections and guidelines outlined in the "Recommendation of the Finnish National Board on Research Integrity TENK 2020" document. Placeholders are included for sections where content is yet to be fully populated, ensuring the structure remains consistent with the template.

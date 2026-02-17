# Gemini Project: Awesome CV

This directory contains a LaTeX project for generating a Curriculum Vitae (CV) and a résumé using the "Awesome CV" template.

## Directory Overview

This is a non-code project focused on creating professional documents using LaTeX. The main components are the `.tex` files, which define the structure and content of the CV and résumé, and the `.cls` file, which provides the styling.

## Key Files

*   **`cv.tex`**: The main file for the Curriculum Vitae. It is a self-contained document with all the content in one file.
*   **`resume.tex`**: The main file for the résumé. It is a modular document that includes content from the `resume/` directory.
*   **`coverletter.tex`**: A LaTeX file for creating a cover letter.
*   **`awesome-cv.cls`**: The LaTeX class file that defines the styles, commands, and layout for the "Awesome CV" template.
*   **`cv/` directory**: Contains the different sections of the CV as separate `.tex` files.
*   **`resume/` directory**: Contains the different sections of the résumé as separate `.tex` files.
*   **`fonts/` directory**: Contains the fonts used in the documents.
*   **`README.md`**: The original README file for the "Awesome CV" template.

## Usage

To generate the CV or résumé, you need to have a full TeX distribution installed on your system (e.g., TeX Live).

You can compile the documents using the `xelatex` command:

*   **To compile the CV:**
    ```bash
    xelatex cv.tex
    ```

*   **To compile the résumé:**
    ```bash
    xelatex resume.tex
    ```

*   **To compile the cover letter:**
    ```bash
    xelatex coverletter.tex
    ```
This will generate `cv.pdf`, `resume.pdf`, and `coverletter.pdf` respectively.

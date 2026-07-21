# Curriculum vitae source

This directory contains the XeLaTeX source exported from the Overleaf project.
The source of truth for the downloadable PDF is `main.tex` and the files in
`sections/`.

## Updating the CV

1. Edit the CV in Overleaf, or edit the matching files here.
2. Export the updated `.tex` files from Overleaf into this directory.
3. Keep `_data/cv.yml` in sync because the website's HTML CV uses that file.
4. Push to `main`. GitHub Actions compiles `cv/main.tex` with XeLaTeX and
   updates `assets/pdf/Pildoo_Sung_CV_2026.pdf` automatically.

The current integration is one-way from the repository to the website. A
direct two-way Overleaf sync can be added later if the Overleaf Git URL and
authentication are configured.

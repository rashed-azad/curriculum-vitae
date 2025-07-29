# Installing LaTeX on Debian 11 and Building PDF

## Installing LaTeX

To install LaTeX with the necessary packages on Debian 11, run the following command:

```bash
sudo apt install texlive-latex-extra texlive-fonts-recommended texlive-latex-recommended texlive-fonts-extra texlive-bibtex-extra -y
```

## Steps to Generate the PDF

### Run the `Makefile`

After creating the `Makefile`, use the following command to build the PDF with a dynamically generated filename:

```bash
make
```

This will compile the LaTeX file `cv.tex`, and the output will be saved as `cv_YYYY-MM-DD_HH-MM-SS.pdf` inside the `build` directory.
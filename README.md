
# LaTeX Installation Guide for MacBook

This guide provides step-by-step instructions to install LaTeX on macOS using Homebrew, TinyTeX, and TeX Live packages.

---

## 1. Install `wget` using Homebrew

`wget` is a useful utility to download files from the internet.

```bash
brew install wget
````

---

## 2. Install TinyTeX

TinyTeX is a lightweight, portable, cross-platform LaTeX distribution.

```bash
curl -sL "https://yihui.org/tinytex/install-unx.sh" | sh
```

---

## 3. Install TeX Live Packages

After installing TinyTeX, you can install additional LaTeX packages using `tlmgr`:

```bash
tlmgr install --reinstall --force \
lbox xcolor pdfx fontspec titlesec enumitem hyperref fontawesome5 everyshi oberdiek \
kvsetkeys kvrprofiles xmpincl accsupp cmap ragged2e pgf tcolorbox tikzfill iftex \
pdfescape ltxcmds pdftexcmds refcount gettitlestring kvoptions stringenc intcalc \
url bitset rerunfilecheck l3packages geon-fontsrecommended tools environ adjustbox \
dashrule ifmtarg multirow changepage paracol lato fo biblatex-ieee epstopdf-pkg \
trimspaces collectbox logreq
```

> This command ensures that all the commonly used LaTeX packages are installed and up to date.
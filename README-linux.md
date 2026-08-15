# LaTeX Setup (TinyTeX)

Self-contained, no `sudo` needed. Lives entirely in `~/.TinyTeX`.

## Install

```bash
wget -qO- "https://yihui.org/tinytex/install-unx.sh" | sh
echo 'export PATH="$HOME/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## Install packages

```bash
tlmgr install collection-basic
tlmgr install --reinstall --force \
lbox xcolor pdfx fontspec titlesec enumitem hyperref fontawesome5 everyshi oberdiek \
kvsetkeys kvrprofiles xmpincl accsupp cmap ragged2e pgf tcolorbox tikzfill iftex \
pdfescape ltxcmds pdftexcmds refcount gettitlestring kvoptions stringenc intcalc \
url bitset rerunfilecheck l3packages tools environ adjustbox \
dashrule ifmtarg multirow changepage paracol lato fo biblatex-ieee epstopdf-pkg \
trimspaces collectbox logreq extsizes fontaxes biblatex biber raleway roboto carlito
```

If a build still errors with `File 'X' not found`:

```bash
tlmgr install <package-name>
```

## VS Code

```bash
code --install-extension James-Yu.latex-workshop
```

## Build

```bash
latexmk -pdf main.tex
```

## Uninstall

```bash
rm -rf ~/.TinyTeX ~/bin
```
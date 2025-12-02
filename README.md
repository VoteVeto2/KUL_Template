# KU Leuven LaTeX Template

A LaTeX template for KU Leuven research proposals/theses with official styling.

## Folder Structure

```
├── main.tex          # Main document (compile this)
├── titlepage.tex     # Title page with KU Leuven branding
├── appendix.tex      # Appendix content
├── references.bib    # Bibliography file
├── logo.pdf          # KU Leuven logo
├── Chapter/          # Chapter files
│   ├── Ch1.tex
│   ├── Ch2.tex
│   ├── Ch3.tex
│   └── Ch4.tex
└── image/            # Images folder
```

## Usage

1. Edit `titlepage.tex` to update your title, name, and supervisor info
2. Write your content in `Chapter/Ch1.tex` through `Chapter/Ch4.tex`
3. Add references to `references.bib`
4. Place images in the `image/` folder
5. Compile `main.tex` with a LaTeX compiler (requires `biber` for bibliography)

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

## Overleaf Setup

To work remotely and collaborate with your team:

1. Download this file as a ZIP  
2. Go to [Overleaf](https://www.overleaf.com)  upload contents to your Overleaf project
3. Change compiler to `LuaLaTeX` (Menu → Settings → Compiler)
4. Click the **Share** button to invite collaborators via email or link

## Features

- KU Leuven blue color scheme
- Palatino body + Helvetica headers
- Author-year citation style with colored hyperlinks
- Gantt chart support (`pgfgantt`)

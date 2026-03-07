<div align="center">
  <p>
    English |
    <a href="./README.zh-CN.md">简体中文</a>
  </p>
  <img src="./fig/S.H.I.T.png" alt="SHIT Journal Template" width="240">
  <h1>SHIT Journal LaTeX Template</h1>
  <p><strong>S.H.I.T. = Sciences · Humanities · Information · Technology</strong></p>
  <p>
    A bilingual academic article template for the fictional journal <strong>SHIT / 构石</strong>
  </p>
  <p>
    <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-blue.svg">
    <img alt="Engine: XeLaTeX" src="https://img.shields.io/badge/engine-XeLaTeX-0F6CBD.svg">
    <img alt="Bibliography: Nature" src="https://img.shields.io/badge/bibliography-Nature-orange.svg">
    <img alt="Language: Chinese + English" src="https://img.shields.io/badge/language-Chinese%20%2B%20English-green.svg">
    <img alt="Status: Available" src="https://img.shields.io/badge/status-Available-success.svg">
  </p>
  <p>
    <a href="#about">About</a> •
    <a href="#features">Features</a> •
    <a href="#quick-start">Quick Start</a> •
    <a href="#build">Build</a> •
    <a href="#license">License</a>
  </p>
</div>

---

## About

This repository contains the LaTeX template for the fictional journal **SHIT / 构石**.
It is designed to provide a compact, journal-like manuscript workflow with bilingual support, a customized title page, structured abstract blocks, standard cross-references, and a Nature-style bibliography setup.

---

## Features

### Journal-style front page

- Custom SHIT masthead and metadata block
- Subject section line and abstract separator rules
- Title, authors, affiliations, abstract, and editorial metadata arranged in a journal layout

### Writing-ready manuscript structure

- `Introduction`
- `Related Work`
- `Methods`
- `Results`
- `Discussion`
- `Conclusion`

### Standard academic components

- Figure example with `./fig/` asset convention
- Table example
- Equation example
- Pseudocode example using `algorithm` + `algpseudocode`
- AI statement block similar to publisher disclosure sections
- Cross-reference examples for figures, tables, algorithms, and equations

### Citation workflow

- Bibliography data stored in `references.bib`
- Nature-style references via `biblatex + biber`
- Blue superscript citation numbers in the main text

---

## Repository Layout

```text
SHIT/
├─ fig/                # manuscript and README image assets
│  ├─ S.H.I.T.png
├─ references.bib
├─ shit_journal_template.tex
├─ README.md
├─ README.zh-CN.md
├─ LICENSE
└─ .gitignore
```

---

## Quick Start

1. Edit `shit_journal_template.tex`.
2. Put manuscript figures into `./fig/`.
3. Maintain references in `references.bib`.
4. Build with XeLaTeX and Biber.

---

## Build

```bash
xelatex shit_journal_template.tex
biber shit_journal_template
xelatex shit_journal_template.tex
xelatex shit_journal_template.tex
```

If your editor still shows an old preview after rebuilding, refresh the PDF viewer manually.

---

## Writing Rules

- Chinese text is configured for `SimSun`.
- English text is configured for `Times New Roman`.
- The main figure folder for the template is `./fig/`.
- Bibliography entries should be maintained in `references.bib`.
- Default citation commands are mapped to Nature-style blue superscripts.

---

## License

This project is released under the **MIT License**.  
See [LICENSE](./LICENSE) for details.

---

<div align="center">
  <sub><i>"Truth Fades, S.H.I.T Lasts."</i></sub>
  <br>
  <sub><i>"真理会过时，构石永恒。"</i></sub>
</div>

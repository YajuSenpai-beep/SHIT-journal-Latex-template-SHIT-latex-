# SHIT Journal LaTeX Template

LaTeX template for the fictional journal `SHIT` (`Sciences Humanities Information Technology`, Chinese title: `构石`).

This template is based on `ctexart` and is configured for bilingual academic writing with:

- English text in `Times New Roman`
- Chinese text in `SimSun`
- Nature-style bibliography via `biblatex + biber`
- Blue superscript citations in the main text
- Standard examples for figures, tables, equations, algorithms, acknowledgements, AI statement, funding, and references

## Files

- `shit_journal_template.tex`: main manuscript template
- `references.bib`: bibliography database
- `fig/`: figure directory used by the template

## Compile

Use XeLaTeX and Biber:

```bash
xelatex shit_journal_template.tex
biber shit_journal_template
xelatex shit_journal_template.tex
xelatex shit_journal_template.tex
```

## Notes

- Put all figure files under `./fig/`.
- The sample figure in the template loads `./fig/example-figure.pdf` if it exists.
- Bibliography entries should be maintained in `references.bib`.
- Default citation commands are configured as Nature-style blue superscripts.

## License

This repository is released under the MIT License. See `LICENSE`.

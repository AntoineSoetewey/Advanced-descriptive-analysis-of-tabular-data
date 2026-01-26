# Advanced Descriptive Analysis of Tabular Data

Comprehensive Quarto book on advanced descriptive analytics for tabular data, aimed at researchers, practitioners, policymakers, data journalists, and graduate students. The material emphasizes interpretable, visual, and applied methods for uncovering structure, associations, and patterns in multivariate datasets.

## Project Structure

- [index.qmd](index.qmd): Preface and front matter
- [about.qmd](about.qmd): Information about the authors
- Foundations: [chapter-00-introduction.qmd](chapter-00-introduction.qmd), [chapter-01-beyond-basic-descriptives.qmd](chapter-01-beyond-basic-descriptives.qmd), [chapter-02-data-types-associations.qmd](chapter-02-data-types-associations.qmd)
- Association Analysis: [chapter-03-association-measures.qmd](chapter-03-association-measures.qmd), [chapter-04-correlation-extensions.qmd](chapter-04-correlation-extensions.qmd), [chapter-05-network-representations.qmd](chapter-05-network-representations.qmd)
- Interactive Visual Analytics: [chapter-06-shiny-exploration.qmd](chapter-06-shiny-exploration.qmd), [chapter-07-association-explorer.qmd](chapter-07-association-explorer.qmd), [chapter-08-communication-visualization.qmd](chapter-08-communication-visualization.qmd)
- Tree-Based Methods: [chapter-09-regression-trees.qmd](chapter-09-regression-trees.qmd), [chapter-10-classification-trees.qmd](chapter-10-classification-trees.qmd), [chapter-11-ensemble-methods-description.qmd](chapter-11-ensemble-methods-description.qmd)
- Interpretable ML: [chapter-12-interpretable-ml-overview.qmd](chapter-12-interpretable-ml-overview.qmd), [chapter-13-feature-importance.qmd](chapter-13-feature-importance.qmd), [chapter-14-partial-dependence.qmd](chapter-14-partial-dependence.qmd), [chapter-15-shapley-values.qmd](chapter-15-shapley-values.qmd)
- AutoML: [chapter-16-automl-descriptive.qmd](chapter-16-automl-descriptive.qmd), [chapter-17-automated-feature-engineering.qmd](chapter-17-automated-feature-engineering.qmd)
- Case Studies: [chapter-18-case-study-policy.qmd](chapter-18-case-study-policy.qmd), [chapter-19-case-study-health.qmd](chapter-19-case-study-health.qmd), [chapter-20-case-study-business.qmd](chapter-20-case-study-business.qmd)
- Back matter: [chapter-21-conclusion.qmd](chapter-21-conclusion.qmd), [references.qmd](references.qmd)
- Configuration: [_quarto.yml](_quarto.yml), [references.bib](references.bib), [LICENSE](LICENSE)
- Outputs: `_book/` (generated HTML/PDF/EPUB)

## Requirements

- Quarto (latest release) — install from <https://quarto.org>
- R (4.2+) with required packages (e.g., `tidyverse`, `rpart`, `partykit`, `iml`, `h2o`, `corrr`, `energy`, `minerva`, `igraph`, `ggraph`, `shiny`)
- Optional: LaTeX distribution for PDF builds

## Build and Preview

- Preview a single chapter (faster during drafting):

	```
	quarto preview chapter-00-introduction.qmd
	```

- Preview the full book (serves HTML to a local port):

	```
	quarto preview
	```

- Render all formats (HTML, PDF, EPUB) as configured in [_quarto.yml](_quarto.yml):

	```
	quarto render
	```

Outputs are written to `_book/`. If PDF fails, ensure a LaTeX distribution is installed (TinyTeX or TeX Live).

## Contributing

1. Fork or create a feature branch.
2. Edit the relevant `.qmd` files; keep prose concise and add citations to [references.bib](references.bib) where appropriate.
3. Run `quarto preview` to check formatting and cross-references.
4. Open a pull request describing the changes and any new dependencies or datasets.

## License

This project is licensed under the terms of [LICENSE](LICENSE). Please attribute the authors when reusing text or code.

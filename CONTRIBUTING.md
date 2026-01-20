# Contributing to Advanced Descriptive Analysis of Tabular Data

Thank you for your interest in contributing to this book! Whether you're fixing typos, improving explanations, adding examples, or suggesting new content, your contributions are welcome.

## Ways to Contribute

### Reporting Issues

If you find errors, unclear explanations, broken code, or have suggestions for improvement:

1. Check the [Issues](https://github.com/AntoineSoetewey/Advanced-descriptive-analysis-of-tabular-data/issues) page to see if it's already reported
2. If not, create a new issue with:
   - A clear, descriptive title
   - The chapter/section where the issue occurs
   - A detailed description of the problem
   - If applicable, suggestions for how to fix it

### Suggesting Content

For suggestions about new topics, examples, or datasets:

1. Open an issue labeled "enhancement" or "content suggestion"
2. Explain what you'd like to see and why it would be valuable
3. If possible, provide references or examples

### Contributing Code or Text

For direct contributions (typo fixes, code improvements, new examples):

1. Fork the repository
2. Create a feature branch
3. Make your changes following the guidelines below
4. Commit with clear messages
5. Push to your fork
6. Open a Pull Request with a description of your changes

## Contribution Guidelines

### Writing Style

- **Audience**: Write for researchers, practitioners, policymakers, and Master-level students
- **Tone**: Professional but accessible; avoid unnecessary jargon
- **Clarity**: Prioritize clear explanations over technical sophistication
- **Active voice**: Prefer active over passive voice
- **Conciseness**: Be thorough but concise; eliminate redundancy

### Technical Writing Standards

- Use **bold** for emphasis and key concepts
- Use *italics* for technical terms on first use
- Use `inline code` for variable names, function names, and short code snippets
- Use numbered lists for sequential steps, bullet points for non-sequential items
- Include cross-references using Quarto syntax: `@sec-label` for sections, `@fig-label` for figures
- Define acronyms on first use: "Principal Component Analysis (PCA)"

### Code Standards

All R code should:

- Follow the [tidyverse style guide](https://style.tidyverse.org/)
- Include comments explaining non-obvious operations
- Use meaningful variable names
- Be reproducible (set seeds where randomness is involved)
- Include package loading at the beginning of chapters
- Work with the versions specified in the book's requirements
- Be tested to ensure it runs without errors
- Be formatted for readability (indentation, spacing)
- Comment on the purpose of code blocks

**Example:**

```r
# Load required packages
library(ggplot2)
library(dplyr)

# Set seed for reproducibility
set.seed(42)

# Create example dataset
data <- tibble(
  x = rnorm(100),
  y = 2 * x + rnorm(100, sd = 0.5)
)

# Visualize relationship
ggplot(data, aes(x = x, y = y)) +
  geom_point() +
  geom_smooth(method = "lm") +
  theme_minimal()
```

### Code Chunks

Use appropriate chunk options:

```r
#| label: fig-example
#| fig-cap: "Descriptive caption"
#| echo: true
#| warning: false
#| message: false
```

- `label`: Descriptive label for cross-referencing
- `fig-cap`: Clear figure caption
- `echo`: Show code (usually `true` for teaching material)
- `warning`/`message`: Suppress unless pedagogically relevant

### Mathematical Notation

- Use LaTeX notation for equations: `$x^2$` for inline, `$$` blocks for display
- Define variables before using them in equations
- Explain the intuition behind formulas, not just the mechanics

### Citations and References

- Add references to `references.bib` in BibTeX format
- Cite using `@key` for in-text citations or `[@key]` for parenthetical
- Include DOIs when available
- Prefer peer-reviewed sources, official documentation, or authoritative textbooks

### Datasets

When adding new datasets or examples:

- Use publicly available datasets when possible
- Provide clear data sources and citations
- Include code to load/download the data
- Ensure data complies with licensing and privacy requirements
- Prefer datasets that illustrate real applied problems

## File Organization

- **Chapter files**: `chapter-##-descriptive-name.qmd`
- **Images**: Place in `images/` directory (create if needed)
- **Data**: Place in `data/` directory or provide download links
- **Supplementary code**: Consider creating `code/` directory for longer scripts

## Building and Testing

Before submitting a PR:

1. **Preview your changes locally:**
   ```bash
   quarto preview chapter-##-yourfile.qmd
   ```

2. **Check that the full book renders without errors:**
   ```bash
   quarto render
   ```

3. **Verify cross-references and citations work**

4. **Test all code chunks execute successfully**

5. **Check for typos and formatting issues**

## Pull Request Process

1. **Title**: Use a clear, descriptive title
2. **Description**: Explain what changes you made and why
3. **Checklist**: Confirm you've:
   - Previewed your changes locally
   - Tested code chunks
   - Followed style guidelines
   - Updated relevant sections (e.g., added references to `.bib`)
4. **Link issues**: Reference related issues using `#issue-number`

## Types of Contributions We're Looking For

### High Priority

- Typo and grammatical error corrections
- Broken code fixes
- Clarifications of confusing explanations
- Additional real-world examples
- Improved visualizations

### Medium Priority

- New exercises or practice problems
- Enhanced code comments
- Alternative approaches to examples
- Performance improvements in code
- Accessibility improvements (alt text, color-blind friendly palettes)

### Lower Priority (Discuss First)

- Major structural changes
- New chapters or sections
- Significant content additions
- Changes to book philosophy or scope

For lower priority items, please open an issue for discussion before investing time in implementation.

## Code of Conduct

### Be Respectful

- Use welcoming and inclusive language
- Respect differing viewpoints and experiences
- Accept constructive criticism gracefully
- Focus on what's best for the community and the book

### Be Professional

- Keep discussions focused on content and technical merit
- Avoid personal attacks or inflammatory language
- Assume good faith from other contributors

### Be Collaborative

- Help newcomers get started
- Share knowledge and expertise
- Credit others' contributions

## Questions?

If you have questions about contributing:

- Open an issue labeled "question", or start a discussion
- Check existing issues and pull requests for similar discussions

## License

By contributing to this project, you agree that your contributions will be licensed under the same license as the project (see [LICENSE](LICENSE)).

---

Thank you for helping make this book better! Your contributions, no matter how small, are valuable to the community.

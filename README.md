# vinayakkgarg.github.io

Personal website of Vinayakk Garg, built with [Quarto](https://quarto.org/) and published via GitHub Pages.

## Contents

- `index.qmd` — about / landing page
- `projects.qmd` + `projects/` — projects organized by area (Computer Vision, NLP, Time-series, Robotics, Kaggle)
- `blog.qmd` — blog posts
- `publications.qmd` + `publications/` — publications
- `highlights.qmd` — highlights page
- `_quarto.yml` — site configuration (navbar, sidebar, theme)

## Local development

Requires [Quarto](https://quarto.org/docs/get-started/) installed.

```bash
# Preview the site locally with live reload
quarto preview

# Render the static site to _site/
quarto render
```

The rendered output in `_site/` is what gets published to GitHub Pages.

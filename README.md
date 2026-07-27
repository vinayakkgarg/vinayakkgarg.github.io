# vinayakkgarg.github.io

Personal website of Vinayakk Garg — Senior ML Engineer. A static site built on the
[iPortfolio](https://bootstrapmade.com/iportfolio-bootstrap-portfolio-websites-template/)
Bootstrap template, served directly by GitHub Pages.

## Structure

```
index.html              single-page site: hero, about, stats, skills,
                        experience, projects, publications, highlights, blog, contact
project-*.html          13 project detail pages, one per project
images/                 profile photo and project images
assets/css/main.css     template stylesheet (unmodified)
assets/css/custom.css   colour theme + all custom sections
assets/js/main.js       template behaviour (nav, scrollspy, lightbox, filters)
assets/vendor/          only the libraries actually used, see below
```

## Local preview

No build step — the site is plain HTML.

```bash
python3 -m http.server 8899
# then open http://localhost:8899/
```

## Theming

Colours are driven entirely by CSS custom properties. The theme block at the top of
`assets/css/custom.css` redefines them; `main.css` is left untouched. The accent
deliberately differs per surface — a darker teal on light sections and a lighter teal
on dark ones — so text keeps a WCAG AA contrast ratio in both.

## Vendor libraries

Only what the page actually uses is committed:

| Library | Used for |
| --- | --- |
| bootstrap (CSS only) | grid and layout utilities |
| bootstrap-icons | all icons |
| aos | scroll reveal animations |
| purecounter | animated stat counters |
| glightbox | project image lightbox |
| isotope-layout + imagesloaded | project grid filtering |

Removed as unused: `typed.js`, `swiper`, `waypoints`, `php-email-form`, and Bootstrap's
JS bundle. The matching dead code was also removed from `main.js`, so the shipped
libraries and the code that calls them stay in sync.

The contact form was replaced with direct links — GitHub Pages cannot execute the
template's PHP handler.

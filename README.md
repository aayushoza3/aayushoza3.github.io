# aayushoza3.github.io

Source for my academic website, built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

## Where to edit

| What | File |
| --- | --- |
| Landing page bio, address, photo settings | `_pages/about.md` |
| Headshot | `assets/img/prof_pic.jpg` |
| Research page | `_pages/research.md` |
| Publications (BibTeX) | `_bibliography/papers.bib` |
| CV | `_data/cv.yml` |
| Social and academic profile links | `_data/socials.yml` |
| News items on the landing page | `_news/` |
| Site name, URL, global settings | `_config.yml` |

Pushing to `main` runs `.github/workflows/deploy.yml`, which builds the site and publishes it to the `gh-pages` branch.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

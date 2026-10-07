# sparql-anything.cc

Website of the SPARQL Anything project: https://sparql-anything.cc

A single-page Jekyll site, built by GitHub Pages. No theme, no JavaScript framework: one stylesheet (`css/site.css`) and a small inline script for the format tabs, the mobile menu and code colouring.

## Updating content

Most updates are data edits, no HTML needed:

| What | Where |
| --- | --- |
| Current release (version, date, Java version) | `release:` in `_config.yml` |
| Current Façade-X specification release | `spec:` in `_config.yml` |
| News items | `_data/news.yml` (newest first, six shown) |
| Publications and BibTeX | `_data/publications.yml` (`cite: true` = reference publication) |
| Tutorials and showcases | `_data/tutorials.yml` |
| Supported formats and their docs pages | `_data/formats.yml` |

Page sections live in `_includes/` and are assembled in `_layouts/front.html`.

The example output in the hero (`_includes/hero.html`) and in "Get started" (`_includes/start.html`) was produced with the release named in `_config.yml` (currently 1.3.0). Re-run them when a release changes the Façade-X output.

## Example files

`examples/`, `example1.json`, `example1.csv`, `books.xml` and `exploratoryQuery/` are referenced by URL from the SPARQL Anything documentation and test suite. Do not move or rename them.

## Build

```
bundle exec jekyll serve --config=_config.yml --livereload
```

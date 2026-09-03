# Alesis QuadraVerb Manual (HTML)

A readable HTML transcription of the original **Alesis QuadraVerb** instruction / user’s manual.

**Live site:** [https://tymcode.github.io/quadraverb-docs/](https://tymcode.github.io/quadraverb-docs/)

## Why

I use the QuadraVerb manual as a reference. Online scans of the original booklet are hard to read — the print quality was already soft, and existing scans make that worse. I scanned my own copy, but even those scans weren’t good enough for day-to-day lookup.

## How

1. Built a large custom word list for [`ocrmypdf`](https://ocrmypdf.readthedocs.io/) so OCR would keep instrument / effect vocabulary intact.
2. Ran `ocrmypdf` on the scans.
3. Converted the OCR’d PDF to HTML with [`pandoc`](https://pandoc.org/).
4. Manually cleaned structure, headings, tables, LCD mockups, figures, and CSS so the result paginates cleanly (including when printing from Chrome).

## Contents

| Path | Description |
|------|-------------|
| [`index.html`](index.html) | Landing page for GitHub Pages |
| [`AlesisQuadraVerbUsersManual.html`](AlesisQuadraVerbUsersManual.html) | Full manual |
| [`quadraverb-manual.css`](quadraverb-manual.css) | Stylesheet |
| [`figures/`](figures/) | Panel diagrams and in-manual figures |

## Serving with GitHub Pages

This repo is published from the `main` branch root (includes `.nojekyll`). After enabling Pages on GitHub, the site is available at:

https://tymcode.github.io/quadraverb-docs/

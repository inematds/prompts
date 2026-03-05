# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Portuguese-language educational site about Prompt Engineering ("Engenharia de Prompts 2.0"), built with **MkDocs Material** and deployed to **GitHub Pages**. All content is Markdown under `docs/`. The site serves as a reusable template for courses, workshops, and corporate training.

## Build & Deploy

```bash
# Install dependencies (Python 3.11+)
pip install -r requirements.txt

# Local development server with live reload
mkdocs serve

# Build static site to ./site/
mkdocs build --clean
```

Deployment is automatic: pushing to `main` triggers `.github/workflows/gh-pages.yml`, which builds and deploys to GitHub Pages.

## Architecture

- **`mkdocs.yml`** — Site config, theme settings, and full navigation tree (`nav:`). Any new page must be added here to appear in the site.
- **`docs/`** — All content lives here:
  - `index.md` — Landing page
  - `educacao/` — Education hub and learning tracks (trilhas): `fundamentos.md`, `tecnicas.md`, `avancado-masterclass.md`
  - `modulo*/README.md` — Six course modules (fundamentos through projetos finais)
  - `guia/` — Usage guides (how to use, adapt for enterprises, course model, agents)
  - `templates/` — Reusable templates for courses, workshops, exercises, prompts
  - `exercicios/` — Exercises hub
  - `recursos/` — Static assets (SVG banner, favicon)
  - `styles/theme.css` — Custom CSS overrides
  - `data/` — Historical archive (inventory.json, reference texts); mostly gitignored except `.txt`, `.json`, `.md`
- **`archive/`** — Temporary publish workspace (currently empty)

## Content Conventions

- All content is written in **Brazilian Portuguese (pt-BR)**. Maintain proper accents and Portuguese grammar.
- Markdown extensions enabled: admonition, footnotes, attr_list, md_in_html, toc with permalinks.
- MkDocs Material features in use: navigation tabs, sections, top button, footer, code copy.
- Internal links use relative paths from the `docs/` root (e.g., `modulo1_fundamentos/README.md`).
- The `nav:` in `mkdocs.yml` is the source of truth for site navigation — update it when adding/renaming/moving pages.

## Validation

There is no linter or test suite. To verify changes, run `mkdocs build --clean` and check for warnings about broken links or missing pages.

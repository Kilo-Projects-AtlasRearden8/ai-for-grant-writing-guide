# STATUS

AI for Grant Writing — beginner manual + static HTML site
Built by Asdale Dynamics, LLC (Copyright (c) 2026 Asdale Dynamics, LLC)

## What was built

A beginner-friendly manual for using free AI to write grants, covering finding funders, drafting narratives, budgets, and reports. Includes step-by-step instructions, copy-and-adapt prompts, fill-in templates, a printable checklist, privacy/ethics guidance, and a static HTML version of the site.

### Files (20 total)

Root:
- README.md — overview, ground rules, credit to Asdale Dynamics, LLC, license pointer
- LICENSE — MIT License, copyright line exactly `Copyright (c) 2026 Asdale Dynamics, LLC`

docs/ (manual, Markdown):
- 01-introduction.md
- 02-finding-funders.md
- 03-drafting-narratives.md
- 04-budgets.md
- 05-reports.md
- 06-privacy-ethics.md (never paste donor data; education only)
- checklist.md (printable)
- templates/narrative-template.md
- templates/budget-template.md
- templates/report-template.md

site/ (static HTML, no build step — open site/index.html in any browser):
- index.html — home/landing
- assets/style.css — shared stylesheet
- pages/finding-funders.html
- pages/drafting-narratives.html
- pages/budgets.html
- pages/reports.html
- pages/privacy-ethics.html
- pages/checklist.html

## How to run it

It's plain Markdown and static HTML — nothing to install, no build step.

- Read the manual: open any `docs/*.md` file in a text editor or Markdown viewer.
- Use the site: open `site/index.html` in a web browser. All pages link together; the CSS lives at `site/assets/style.css`.
- Print the checklist: open `docs/checklist.md` or `site/pages/checklist.html` and print.
- Copy templates: `docs/templates/*.md` are fill-in-the-blank starting points.

No server, no dependencies, no accounts, no API keys.

## Verification results

- Custom verification script (Python stdlib only) checked all 20 files.
- LICENSE contains the exact copyright line `Copyright (c) 2026 Asdale Dynamics, LLC`.
- README credits Asdale Dynamics, LLC.
- All internal links in HTML resolve (0 broken links).
- All internal links in Markdown resolve (0 broken links).
- No secrets, API keys, or personal data found in any file.
- No `.github/workflows` present.
- No `node_modules`, build artifacts, or test suite (content-only project; nothing to compile or test beyond link/file checks).

Verification command (re-runnable):
`python3 - <<'PY' ...` — the inline HTML/link checker above; returns no broken links.

## Known gaps

- No automated test framework or CI (intentionally: no `.github/workflows`, no build tooling). Verification is the link/file checker script run manually.
- HTML pages are standalone copies; shared nav/footer are duplicated per page rather than templated (acceptable for a small static site).
- The static site does not include a rendered version of docs/01-introduction.md as a separate page; index.html covers the overview.
- No search function on the static site (site is small enough to navigate via the menu).
- Templates are Markdown text; no pre-formatted PDF/print layouts beyond the printable checklist.

## Credit

Written by Dylan Asdale, registered nurse turned AI author and founder of Asdale Dynamics, LLC (Indiana, formed October 2026). Credit: Asdale Dynamics, LLC. Education only — not legal, financial, or medical advice.

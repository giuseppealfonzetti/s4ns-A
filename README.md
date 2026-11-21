# Statistics for Neuroscience A

Course website (Quarto), PhD in Neuroscience 2026/27.

```
index.qmd                schedule (links only to released material)
sessions/0N-*/           released: slides.qmd, exercises.qmd, solutions.qmd
_drafts/0N-*/            not released: never rendered, not in git
themes/                  UniPD red slide + site themes
data/                    datasets + README (sources/licences)
```

## Release a session

1. Before class: `mkdir -p sessions/0N-x && mv _drafts/0N-x/{slides,exercises}.qmd sessions/0N-x/`
2. In `index.qmd`, fill that row: slides and exercises links.
3. `quarto publish gh-pages`, then commit and push.
4. After class: same for `solutions.qmd`.

Preview a draft: `quarto preview _drafts/0N-x/slides.qmd` (output stays in `_drafts/`). Commit `_freeze/`.
Slides to PDF: press `E`, then print.

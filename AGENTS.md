# Project instructions

This repository contains the public Quarto blog at
`https://chrwittm.github.io/`.

## Start of every session

- Read `_maintenance/BACKLOG.md` before starting maintenance or structural
  work.
- Check `git status` and preserve unrelated user changes.
- Treat `main` as the source branch and `gh-pages` as generated deployment
  output.

## Publication safety

- Do not run `quarto publish`, push a branch, or change `gh-pages` unless the
  user explicitly requests it.
- Do not edit generated files in `_site/` as source files.
- Keep the explicit `project.render` allowlist in `_quarto.yml`. New public
  pages must be added deliberately.
- A post's canonical public source is `posts/YYYY-MM-DD-slug/index.qmd` or
  `posts/YYYY-MM-DD-slug/index.ipynb`.
- New posts should begin with `draft: true` and should not be published until
  the user explicitly approves publication.

## Content and privacy

- Preserve the author's voice and existing article content unless a change is
  requested.
- Before drafting or substantially revising a blog post, read and follow
  `_editorial/voice-and-style.md`. Treat it as the default editorial guide while
  giving the user's instructions and the specific post's purpose precedence.
- This is a public repository. Never commit secrets, private source material,
  personal data, or credentials. Remember that notebook outputs are public too.
- Material intended only for local use belongs in an ignored `.private/`
  directory once that convention has been implemented.

## Maintenance workflow

- Work on one backlog item, or one tightly related group, at a time.
- Give maintenance changes focused commits and verify them before publication.
- Update `_maintenance/BACKLOG.md` when an item's status, scope, evidence, or
  completion state changes.
- Record newly discovered work in the backlog instead of silently expanding the
  current task.

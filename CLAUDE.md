# CLAUDE.md

## Repo

This is a static personal website hosted on GitHub Pages at https://akshaybalwally.github.io.

## Rules

- Before any push, update the "last updated" date in `index.html` to today's date if any content has changed.
- When the user asks to "update my projects", scan all public GitHub repos using `gh repo list akshaybalwally --json name,description,url,pushedAt`, then update the Projects section in `index.html`:
  - Each project gets a grey date line (class `project-date`) showing the date of the last commit, and a description below it.
  - Projects are ordered by last commit date, most recent first.
  - Exclude the `akshaybalwally.github.io` repo itself.
  - For new repos, investigate the README/source to write a 1-2 sentence description.

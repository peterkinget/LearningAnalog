# Notes for AI agents

Learning Analog is a Jupyter Book (1.x) published at https://learninganalog.com.
See `WORKFLOW.md` for the human edit/build/publish routine.

## Layout

- `_config.yml`, `_toc.yml` — book configuration and table of contents.
  `only_build_toc_files: true`, so a page must be in `_toc.yml` to be built.
- `intro.md` — landing page; content lives under `TestYourKnowledge/`.
- `_build/` — build output, ignored by git.
- `venv_jupyterbook/` — local Python environment, ignored by git;
  create from `requirements.txt` if missing.

## Building

```
venv_jupyterbook/bin/jupyter-book clean . ; venv_jupyterbook/bin/jupyter-book build .
```

Report any warnings. Do not upgrade to Jupyter Book 2.x.

## Rules

- The owner reviews changes before they leave this machine:
  commit locally, but ask before `git push`.
- **Never publish**: do not run `ghp-import` or modify the `gh-pages`
  branch. The owner publishes.
- Plan and ask before large restructurings (moving or renaming pages
  changes public URLs).
- Do not commit `_build/`, `venv_jupyterbook/`, `.DS_Store`, or
  `.ipynb_checkpoints/`.

## Known issues

- `_config.yml` `repository:` says `path_to_book: docs` and
  `branch: master`; the book is at the repo root on `main`.

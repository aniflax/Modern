# AGENTS — Modern

## Workflow Rule — Auto Commit & Push

**Every change in any folder must be committed and pushed to GitHub immediately.**

- Scope: **all folders** — `modern/`, `arkit/`, root, and any new folder/file.
- Action: after any file creation, edit, deletion, or rename:
  1. `git add -A`
  2. `git commit -m "<concise description of change>"`
  3. `git push origin main` (current branch is `main` → `origin/main` at `git@github.com:aniflax/Modern.git`)
- Do not batch unrelated changes — commit per logical change and push before starting next task.
- Do not leave uncommitted or unpushed changes at end of session.
- If push fails (auth/network/conflict), resolve before continuing and report status.

## Project Notes
- Stack: static HTML templates — `modern/` (Modern) and `arkit/` (Arkit).
- No build step — direct HTML/CSS/JS edits.
- Keep navigation and asset paths consistent across homepage variants (`index.html`, `index-2.html`, etc.).

## Agent Instructions
- Read this file at session start.
- Verify `git status` before and after every change set.
- Prefer atomic commits with clear messages (e.g., `feat: add homepage 4 editorial split`).

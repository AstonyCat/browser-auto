# AGENTS.md

## Cursor Cloud specific instructions

This repository (`browser-auto` — 浏览器自动化任务) is currently an empty project with only a `README.md`. There is no source code, no dependency manifest, no build system, and no runnable application yet.

### Current state

- **No services to start** — the repo has no application code.
- **No tests to run** — no test files or test framework configured.
- **No lint/build commands** — no linter or build tool configured.
- **No dependencies to install** — no `package.json`, `requirements.txt`, `pyproject.toml`, or similar files exist.

### When code is added

Once source code and a dependency manifest are added to this repo, the update script and this file should be revised accordingly. Future agents should check for the presence of dependency files (`requirements.txt`, `pyproject.toml`, `package.json`, etc.) and install dependencies as needed.

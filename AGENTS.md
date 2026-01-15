# Repository Guidelines

## Project Structure & Module Organization
This repository currently has no source files committed. When adding code, keep a simple, predictable layout:
- `src/` for application or library code.
- `tests/` for automated tests (mirror `src/` paths).
- `assets/` for static files (images, data files, or reference docs).
- `scripts/` for helper scripts (build, lint, dev).

If a different structure is required, document it in this file and keep paths consistent.

## Build, Test, and Development Commands
No build or test commands are defined yet. When you add tooling, document the exact commands here. Examples to keep in mind:
- `npm run build` for production builds.
- `npm test` or `pytest` for running tests.
- `npm run dev` or `python -m ...` for local development.

## Coding Style & Naming Conventions
- Indentation: 2 spaces for YAML/JSON; 4 spaces for Python; match language defaults when added.
- Filenames: use `kebab-case` for scripts (e.g., `build-assets.ps1`) and `snake_case` for Python.
- Add formatter/linter configs (e.g., `.editorconfig`, `prettier`, `ruff`) as soon as a language stack is chosen.

## Testing Guidelines
No test framework is configured yet. When introducing tests, specify:
- Framework (e.g., `pytest`, `jest`).
- Coverage expectations (if any).
- Naming conventions (e.g., `test_*.py`, `*.spec.ts`).

## Commit & Pull Request Guidelines
There is no Git history yet, so no established convention. Use clear, imperative commit messages and consider Conventional Commits (e.g., `feat: add room planning model`).
Pull requests should include:
- A short description of changes and rationale.
- Linked issues or tasks if applicable.
- Screenshots or sample output for UI or report changes.

## Configuration & Secrets
Do not commit secrets. Store local configuration in `.env` or a similar ignored file, and document required keys in `README.md` once defined.

<!--
Short, actionable instructions for AI coding agents working in this repository.
Keep this file concise (20–50 lines). Update when repository adds source code or CI.
-->

# copilot-instructions

Purpose: help an AI quickly become productive in this repo by describing what is present, where to look, and which concrete steps to take when asked to implement or modify behavior.

Summary of what's in this repository (discoverable):
- `README.md` — project title: "jlpt" (Japanese Language Proficiency Test). No source code, build or test manifests were found at time of inspection.
- `LICENSE` — project license file.

Quick orientation (big picture):
- This repo currently contains only documentation-level files. There are no language-specific source folders (no `src/`, no `package.json`, no `pyproject.toml`, no `pom.xml`, etc.).
- If asked to implement features, expect to create appropriate language layout and manifest files and update `README.md` to document build/run/test steps.

Concrete discovery checklist (what an agent should run first):
1. Look for language or build manifests in repo root: `package.json`, `requirements.txt`, `pyproject.toml`, `setup.py`, `Pipfile`, `pom.xml`, `build.gradle`, `go.mod`.
2. Check for CI/workflow files under `.github/workflows/` and any existing tests under `tests/`, `spec/`, or `__tests__/`.
3. If none exist, surface this in the PR and include suggested scaffolding (minimal `README` updates + manifest + test harness).

Developer workflows (how an AI should behave, given current repo state):
- Do not assume a language. Detect it by presence of manifest files. If none, ask the user which language/environment to use.
- When adding code, also add minimal documentation in `README.md` describing how to build, run, and test the new code.
- Use feature branches for changes (e.g., `feat/<short-desc>`), include a short PR description, and list the files added/changed.

Examples and templates (what to produce or look for):
- If you add Python: create `pyproject.toml` or `requirements.txt`, `src/` and `tests/`, and a short README section with commands such as:
  - `python -m venv .venv` then `pip install -r requirements.txt` and `pytest` to run tests.
- If you add Node: create `package.json`, `src/`, and `test/`; include `npm test` and `npm install` in README.

Project-specific conventions (observed / required):
- None enforced by files in the repository today. Follow common conventions for the chosen language and document them in `README.md` when you add code.

Integration points & external dependencies (discoverable):
- No external integrations or service endpoints are present in the repository files.

When to ask the human: be explicit whenever:
- There is no manifest or language detected and a concrete implementation is requested.
- You intend to add opinionated structure (CI, packaging, or a specific language) — ask what the preferred language/tooling is.

If this file looks incomplete, tell me which language or feature you want implemented and I will update the instructions and scaffold accordingly.

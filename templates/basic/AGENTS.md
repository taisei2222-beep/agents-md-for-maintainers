# Agent Guidelines — [YOUR_PROJECT_NAME]

## Project overview

[Brief description of what this project does and who uses it.]

## Dev environment

```bash
# Clone and install
git clone https://github.com/[YOUR_ORG]/[YOUR_REPO]
cd [YOUR_REPO]
[YOUR_INSTALL_COMMAND]  # e.g. npm install / pip install -e ".[dev]"
```

- Language: [e.g. Python 3.11+ / Node.js 20+]
- Package manager: [e.g. uv / pnpm]
- Main entry point: [e.g. src/index.ts / src/main.py]

## Running tests

```bash
[YOUR_TEST_COMMAND]  # e.g. pytest / npm test
```

All tests must pass before committing. Do not disable or skip tests to make them pass.

## PR guidelines

- Keep PRs focused — one concern per PR
- Write a clear description of what changed and why
- Reference the related issue if one exists: `Fixes #123`
- Do not commit directly to `main`

## Review guidelines

- Flag any change that modifies public API surface without updating docs
- Flag missing or insufficient test coverage
- Flag hardcoded secrets, credentials, or environment-specific paths
- Treat test failures as P0 — never approve a PR with failing tests

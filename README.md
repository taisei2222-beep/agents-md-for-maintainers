# agents-md-for-maintainers

**AGENTS.md templates and GitHub Actions workflows for OSS maintainers.**

Just like `README.md` is written for humans, `AGENTS.md` is written for AI coding agents.  
This repository provides ready-to-use templates and automation workflows so maintainers can immediately integrate Codex into their PR review, issue triage, and release processes.

## Why this exists

Maintaining an OSS project is repetitive work — reviewing PRs, triaging issues, writing release notes.  
Codex can handle a large portion of that, but only if it understands your project's context and rules.  
`AGENTS.md` is how you give Codex that context. This repo gives you battle-tested templates to start from.

## What's included

```
templates/
  basic/          — Minimal AGENTS.md for any project
  python-library/ — Python package with uv, pytest, type hints
  node-package/   — Node.js/TypeScript library with npm/pnpm
workflows/
  codex-pr-review.yml    — Auto-trigger Codex review on PRs
  codex-issue-triage.yml — Label and respond to new issues via Codex
```

## Quick start

1. Pick a template from `templates/` that matches your project
2. Copy it to your repo root as `AGENTS.md`
3. Customize the sections for your stack
4. (Optional) Add a workflow from `workflows/` for full automation

## Templates

| Template | Use case |
|---|---|
| [basic](./templates/basic/AGENTS.md) | Any project — minimal setup |
| [python-library](./templates/python-library/AGENTS.md) | Python packages, uv, pytest |
| [node-package](./templates/node-package/AGENTS.md) | Node.js / TypeScript libraries |

## Contributing

PRs welcome. If you have a template for a stack not covered here, open an issue or submit a PR.

## License

MIT

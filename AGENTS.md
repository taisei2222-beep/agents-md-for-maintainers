# Agent Guidelines

This repository maintains AGENTS.md templates for OSS projects.
Codex is used for PR review, issue triage, and keeping templates up to date.

## Repository structure

- `templates/` — AGENTS.md templates by project type
- `workflows/` — GitHub Actions workflows for Codex automation
- `docs/` — Guides and documentation

## Development environment

No build step required. All files are Markdown or YAML.

To preview Markdown locally, any editor with Markdown preview works (VS Code recommended).

## Contribution guidelines

- Keep templates generic — avoid project-specific assumptions
- Each template must include: Project Overview, Dev Environment, Testing, PR Guidelines, Review Guidelines
- YAML workflows must be tested against a real repository before merging

## PR review guidelines

- Flag any template that hardcodes project-specific paths or commands
- Ensure all placeholders follow the `[YOUR_VALUE]` convention
- Check that Review guidelines section is present in every template
- Treat broken YAML in workflows/ as P0

## Issue triage guidelines

- Label `template-request` for new stack requests
- Label `bug` for broken templates or workflows
- Label `enhancement` for improvements to existing templates

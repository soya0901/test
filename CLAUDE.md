# CLAUDE.md

This file provides guidance for AI assistants (Claude Code and similar tools) working in this repository.

## Repository Overview

A minimal static HTML project. The codebase currently consists of a single entry-point file with no build tooling, dependencies, or framework.

## Repository Structure

```
/
├── index.html      # Single-page HTML entry point
└── CLAUDE.md       # This file
```

## Codebase Details

### index.html

A bare-bones HTML5 document:

- DOCTYPE: `HTML5`
- Language: `en-US`
- Charset: `UTF-8`
- No external stylesheets, scripts, or assets referenced
- No JavaScript
- Body contains a single `<p>test</p> ` placeholder

## Development Workflow

### Branching

- The default branch is `master`.
- Feature/AI branches follow the pattern `claude/<description>-<SESSION_ID>` (e.g., `claude/add-claude-documentation-C4M7P`).
- Always develop on the designated feature branch; never push directly to `master` without explicit permission.

### Making Changes

1. Confirm you are on the correct feature branch before editing any file.
2. Edit files using targeted, minimal changes — avoid unnecessary reformatting or scope creep.
3. Commit with a clear, descriptive message summarising the *why*, not just the *what*.
4. Push with `git push -u origin <branch-name>`.

### Git Conventions

- Commit messages: imperative mood, concise (e.g., `Add navigation bar to index.html`).
- Do not force-push or rebase shared branches without explicit user approval.
- Do not skip hooks (`--no-verify`) unless explicitly instructed.

## Code Conventions

| Convention | Rule |
|---|---|
| HTML standard | HTML5 (`<!DOCTYPE HTML>`) |
| Language attribute | Always set `lang` on `<html>` |
| Charset | Always declare `charset="UTF-8"` in `<head>` |
| Indentation | Tabs |
| External resources | Add only when necessary; prefer CDN-free, self-contained assets for a static project |

## No Build / Test Tooling

This project has **no** package manager, build system, linter, or test suite configured. Until these are introduced:

- Do not run `npm`, `yarn`, `pnpm`, or similar commands.
- Do not create `package.json`, `webpack.config.js`, or similar config files unless explicitly asked.
- Validate HTML manually or with the [W3C Validator](https://validator.w3.org/) if needed.

## Notes for AI Assistants

- Keep changes minimal and focused on what is explicitly requested.
- Do not add frameworks, libraries, or tooling without user approval.
- Do not create new files unless they are strictly necessary.
- If asked to add styling or scripting, prefer inline `<style>` / `<script>` blocks until a more structured approach is agreed upon.
- This is a test/sandbox repository — treat it as a learning or prototyping environment.

# Codex Frontend Skill

A reusable Codex skill for implementing frontend apps, pages, and interactive tools with a practical build-and-verify loop.

## Skill

- `frontend-implementation`: Use when Codex is asked to build, modify, or polish a web frontend, including React/Vite apps, static HTML/CSS/JS pages, dashboards, forms, and browser-based tools.

## Install

Copy the skill folder into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R skills/frontend-implementation ~/.codex/skills/
```

Restart Codex after installing so it can discover the new skill.

## Use

Ask Codex to use the skill explicitly:

```text
Use $frontend-implementation to build this dashboard page and verify it in the browser.
```

Codex can also invoke it automatically when the task matches the skill description.

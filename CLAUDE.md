# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **Claude Code skills repository** — a collection of skill files that extend Claude's capabilities when invoked via the `writing-skills` skill or the `npx skills` CLI.

## Repository Structure

```
skills/
├── CLAUDE.md
└── <skill-name>/
    ├── SKILL.md            # skill definition (YAML frontmatter + instructions)
    └── examples/           # example artifacts produced using the skill
```

Each skill lives in its own directory named after the skill. The skill definition file must be named `SKILL.md` (required by the `npx skills` CLI). The `examples/` subdirectory holds sample outputs or reference materials for that skill.

## Skill File Format

Each skill definition is a Markdown file with YAML frontmatter:

```markdown
---
name: skill-name
description: When to trigger this skill (used by Claude to decide when to invoke it)
metadata:
  category: technique | tool | workflow | ...
  triggers: comma-separated trigger phrases
---

# Skill content in Markdown
```

- The `description` field is critical — it controls when Claude auto-invokes the skill
- `triggers` lists keywords (including non-English) that activate the skill

## Working with Skills

Use the `writing-skills` skill when creating or editing skill files to ensure correct format and deployment.

The `.claude/settings.local.json` pre-approves `Bash(npx skills:*)` commands for skill management.

## Current Skills

| Directory | Skill | Description |
|-----------|-------|-------------|
| `ai-tutorials/` | `ai-tutorials` | Design AI/ML courses via a strict 6-step workflow with user confirmation gates |

# Skills

A personal collection of [Claude Code](https://claude.ai/code) skills.

## Installation

Install all skills from this repo into your project:

```bash
npx skills add https://github.com/likefallwind/skills
```

Install globally (available across all projects):

```bash
npx skills add https://github.com/likefallwind/skills --global
```

Install a specific skill only:

```bash
npx skills add https://github.com/likefallwind/skills --skill ai-tutorials
```

## Available Skills

| Skill | Description |
|-------|-------------|
| `ai-tutorials` | Design AI/ML courses with a structured workflow: knowledge points → syllabus → lectures + projects → self-review → README |

## Updating Skills

Re-run the install command to pull the latest version:

```bash
npx skills add https://github.com/likefallwind/skills
```

If installed globally:

```bash
npx skills add https://github.com/likefallwind/skills --global
```

## Usage

After installation, skills are triggered automatically based on your request. You can also invoke them explicitly:

```
/ai-tutorials
```

## Repo Structure

```
skills/
└── <skill-name>/
    ├── <skill-name>.md   # skill definition
    └── examples/         # reference artifacts
```

# Claude Code Configuration

This directory contains Claude Code configuration for the Forge Providers project.

## Structure

```text
.claude/
├── settings.json     # Claude Code settings
├── rules/            # Project-specific rules
│   └── project.md    # Providers-specific guidelines
├── agents/           # Subagent definitions (add as needed)
├── commands/         # Custom slash commands (add as needed)
└── skills/           # Specialized skills (add as needed)
```

## Inherited Configuration

This project inherits configuration from:
- **Parent:** `compass-forge/CLAUDE.md`
- **Root:** `compass-brand/.claude/rules/`

## Adding Configuration

- **New rules:** Add markdown files to `rules/`
- **Custom commands:** Add markdown files to `commands/`
- **Subagents:** Add markdown files to `agents/`
- **Skills:** Add skill folders to `skills/` with a `SKILL.md` file

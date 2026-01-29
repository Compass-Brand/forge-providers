# CLAUDE.md

This file provides guidance to Claude Code when working in this repository.

## Project: Forge Providers

**Description:** Multi-provider LLM abstraction layer with automatic fallback and cost tracking.

**Project Type:** development

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Language | Python 3.11+ |
| Providers | OpenAI, Anthropic, Ollama |
| Framework | Pydantic |
| Async | asyncio |

---

## Development Methodology: TDD

All functional code MUST follow Test-Driven Development.

```
RED -> GREEN -> REFACTOR
```

---

## Git Discipline (MANDATORY)

**Commit early, commit often.**

- Commit after completing any file creation or modification
- Maximum 15-20 minutes between commits
- Use conventional commit format: `type: description`

Types: `feat`, `fix`, `refactor`, `docs`, `chore`, `test`

# Forge Providers Project Rules

## Project-Specific Guidelines

This project implements a multi-provider LLM abstraction layer with automatic fallback and cost tracking.

### Architecture Principles

- Provider-agnostic interface design
- Failover chains for high availability
- Cost tracking at request level
- Rate limiting with graceful degradation

### Code Organization

- `providers/` - Individual provider implementations (OpenAI, Anthropic, Ollama)
- `core/` - Unified interface and orchestration logic
- `models/` - Pydantic models for requests and responses
- `tracking/` - Cost tracking and metrics collection
- `config/` - Provider configuration and fallback chains

### Provider Implementation

- Each provider must implement the base `LLMProvider` interface
- Handle provider-specific error codes and retry logic
- Normalize responses to common format
- Log all API calls with timing and cost data

### Testing Requirements

- Mock external API calls in unit tests
- Test failover behavior with simulated failures
- Validate cost calculation accuracy
- Test rate limiting edge cases
- Ensure async operations work correctly

### Security Considerations

- Never log API keys or tokens
- Use environment variables for credentials
- Implement request sanitization before logging
- Validate model permissions per provider

## Inherited Rules

This project inherits all rules from:
- `compass-brand/.claude/rules/` (coding style, security, testing, git workflow, performance, agents)
- `compass-forge/CLAUDE.md` (parent project guidelines)

---
name: codex-usage
description: REQUIRED reading before using Codex MCP tools (codex, codex-reply, codex-review). Provides collaboration guidelines for working with OpenAI Codex as an external AI agent. Use when making complex decisions that benefit from a second perspective, validating architectural decisions or implementation plans, reviewing code after significant changes, or brainstorming approaches before committing to a direction.
---

# Codex Collaboration Guidelines

Use OpenAI Codex as a collaborative sub-agent for brainstorming, plan validation, and code review. Treat output as a second opinion—critically evaluate, don't blindly accept.

## Tools

- `codex` — Start new session (defaults to read-only sandbox)
- `codex-reply` — Continue session with prior context
- `codex-review` — Dedicated review mode (fresh session, specialized prompt)

## When to Use

- Complex decisions where a second perspective adds value
- Architectural validation before implementation
- Plan validation before presenting to user
- Code review after significant changes

## When NOT to Use

- Simple, straightforward tasks
- Time-sensitive operations where latency matters
- Trivial changes that don't warrant discussion

## Guidelines

- **Form your own analysis first** to ensure independent perspectives—avoid anchoring bias
- Prompt specifically with context (like any sub-agent)
- Use read-only sandbox unless explicitly required otherwise
- Use `codex-reply` for multi-turn discussions or reviews needing prior context
- Synthesize conclusions—don't just relay raw Codex output
- When developing plans (yourself or via Plan sub-agent), validate with Codex before presenting to user

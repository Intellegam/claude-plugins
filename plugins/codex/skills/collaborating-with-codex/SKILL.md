---
name: collaborating-with-codex
description: Collaborates with OpenAI Codex as an external AI agent for second opinions on complex decisions. Provides guidelines for brainstorming, plan validation, and code review workflows. Use when making architectural decisions, validating implementation plans, reviewing code after significant changes, or consulting codex, codex-reply, or codex-review MCP tools.
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

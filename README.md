# Intellegam Claude Plugins

Internal Claude Code plugins for the Intellegam workspace.

## Marketplace

**Name:** `intellegam-claude-plugins`

## Available Plugins

### codex

OpenAI Codex collaboration MCP server for brainstorming, plan validation, and code review with an external AI agent.

**Includes:**
- MCP server configuration (references `github:Intellegam/codex-mcp`)
- `codex-usage` skill with collaboration guidelines

## Installation

Add the marketplace to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "intellegam-claude-plugins": {
      "source": {
        "source": "github",
        "repo": "intellegam/claude-plugins",
      }
    }
  },
  "enabledPlugins": {
    "codex@intellegam-claude-plugins": true
  }
}
```

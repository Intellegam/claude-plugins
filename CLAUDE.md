# Claude Plugins

Internal Claude Code plugins for the Intellegam workspace.

You MUST read the following file for more information:

- @README.md

## Structure

```
claude-plugins/
├── .claude-plugin/
│   └── marketplace.json    # Marketplace definition with plugin versions
├── plugins/
│   └── <plugin-name>/
│       ├── .claude-plugin/
│       │   └── plugin.json # Plugin metadata (version source of truth)
│       ├── .mcp.json       # MCP server configuration (optional)
│       ├── skills/         # Agent skills (optional)
│       └── hooks/          # Event hooks (optional)
└── README.md
```

## Development

- Plugin versions must be updated in both `plugin.json` and `marketplace.json`
- MCP servers are separate repos (e.g., `codex-mcp`) referenced via GitHub

# Cursor plugins

Cursor plugin test workspace. The active plugin is a standalone directory at the repository root with its own `.cursor-plugin/plugin.json` manifest.

## Plugins

| Plugin | Category | Description |
|:-------|:---------|:------------|
| [teaching-TEST](teaching/) | Utilities | Test-focused skill mapping, practice plans, and feedback loops |

## Repository structure

This workspace currently ships a single plugin. The root `.cursor-plugin/marketplace.json` lists active plugins, and each plugin has its own manifest:

```
plugins/
├── .cursor-plugin/
│   └── marketplace.json       # Marketplace manifest (lists all plugins)
├── plugin-name/
│   ├── .cursor-plugin/
│   │   └── plugin.json        # Per-plugin manifest
│   ├── skills/                # Agent skills (SKILL.md with frontmatter)
│   ├── rules/                 # Cursor rules (.mdc files)
│   ├── mcp.json               # MCP server definitions
│   ├── README.md
│   ├── CHANGELOG.md
│   └── LICENSE
└── ...
```

## License

MIT

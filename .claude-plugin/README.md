## Claude Code marketplace manifest

`marketplace.json` in this folder is the Claude Code plugin marketplace manifest for this
repo. Claude Code reads it when you run `/plugin marketplace add <repo-or-path>`.

Each entry's `source` points to a directory under `./plugins/` (set by `metadata.pluginRoot`).
Every plugin directory carries its own `.claude-plugin/plugin.json`; skills, agents, and MCP
servers are auto-discovered from each plugin's `skills/`, `agents/`, and `.mcp.json`.
# daily.dev marketplace

Agent skills built by the community on the [daily.dev API](https://docs.daily.dev/public-api/)
and approved on the [daily.dev plugin marketplace](https://daily.dev/marketplace).
Every plugin is reviewed by the daily.dev team before it lands here.

## Install

**Claude Code**

```bash
claude plugin marketplace add https://daily.dev/marketplace/claude
claude plugin install <plugin-name>@daily-dev-community
```

**Codex / ChatGPT**

```bash
codex plugin marketplace add dailydotdev/marketplace
```

Then open `/plugins` and pick a plugin from the daily.dev community tab.

**Cursor** (Teams and Enterprise)

Dashboard -> Plugins & MCPs -> Team Marketplaces -> Add Marketplace -> Import from Repo,
then paste `https://github.com/dailydotdev/marketplace`. Turn on Auto Refresh to get new plugins.

Most plugins need a daily.dev API token: create one at https://daily.dev/settings/api,
or connect the [daily.dev MCP server](https://docs.daily.dev/mcp-server/).

## Layout

```
.claude-plugin/marketplace.json     Claude Code
.agents/plugins/marketplace.json    Codex / ChatGPT
.cursor-plugin/marketplace.json     Cursor
plugins/<name>/
  plugin.json                       Agent Plugins manifest (Codex, Cursor)
  .claude-plugin/plugin.json        Claude Code manifest
  skills/<skill>/SKILL.md
```

## How plugins get here

Plugins approved on daily.dev/marketplace that ship a SKILL.md are synced
automatically, one pull request per plugin. To change a plugin, update it on
daily.dev/marketplace; the approved update is synced the same way.

These plugins are written by community members, not by daily.dev. Read a
plugin's SKILL.md before installing it.

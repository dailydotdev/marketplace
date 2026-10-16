# daily.dev community plugins

Agent skills built by the community on the daily.dev API and approved on the
[daily.dev plugin marketplace](https://daily.dev/marketplace). Each plugin is
reviewed by the daily.dev team before it lands here. See the
[Marketplace docs](https://docs.daily.dev/plugin-marketplace/) for how plugins work.

## Install

**Claude Code**

```bash
claude plugin marketplace add https://daily.dev/marketplace/claude
claude plugin install <plugin-name>@daily-dev-community
```

(`claude plugin marketplace add dailydotdev/marketplace` works too.)

**Codex / ChatGPT**

```bash
codex plugin marketplace add dailydotdev/marketplace
```

Then install plugins from the `daily.dev community` marketplace in `/plugins`.

**Cursor** (Teams and Enterprise)

In Dashboard > Plugins & MCPs > Team Marketplaces, choose Import from Repo and
paste `https://github.com/dailydotdev/marketplace`. Turn on Auto Refresh to get
new plugins as they are approved.

## How plugins get here

Approved marketplace plugins that ship a SKILL.md are synced automatically.
`plugins/<name>/` holds the plugin manifests and the skill, and the marketplace
files list them for each agent. Every change goes through a pull request. To
change a plugin, update it on daily.dev/marketplace; the approved update is
synced the same way.

These plugins are written by community so verify plugin's SKILL.md before using
it as you would with any other 3rd party code or prompt.

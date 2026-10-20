# This plugin has moved

> **This repository is superseded.** The Xpoz plugin for Claude Code now lives at
> **[XPOZpublic/xpoz-claude-code-plugin](https://github.com/XPOZpublic/xpoz-claude-code-plugin)**
> and has been submitted to the Claude plugin directory (installs as `xpoz@claude-community` once listed).

The new plugin is a full rebuild on the current Claude Code plugin spec: namespace `xpoz`, OAuth-based connection to the Xpoz MCP server, and three skills (`/xpoz:getting-started`, `/xpoz:social-tracking`, `/xpoz:best-practices` with per-platform references for Twitter/X, Instagram, Reddit, and TikTok).

## Install the current plugin

```bash
git clone https://github.com/XPOZpublic/xpoz-claude-code-plugin.git
claude --plugin-dir ./xpoz-claude-code-plugin
```

Or, once listed in the community marketplace:

```
/plugin marketplace add anthropics/claude-plugins-community
/plugin install xpoz@claude-community
```

## About Xpoz

[Xpoz](https://xpoz.ai) is a social media intelligence platform: search and analyze Twitter/X, Instagram, Reddit, and TikTok (billions of posts) through MCP, with no social media API keys required. Docs: [xpoz.ai/docs](https://xpoz.ai/docs) · Support: support@xpoz.ai

The contents of this repository (March 2026 plugin format) are kept for history and no longer maintained.

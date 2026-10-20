# XPOZ Social Intelligence - Quick Start

Real-time social media analysis for Claude Code. Analyze data from **Twitter/X, Reddit, and Instagram**.

## Step 1: Set Up XPOZ (Do This First!)

1. **Sign up**: Go to [xpoz.ai](https://xpoz.ai?utm_source=claude-code-plugins&utm_medium=github&utm_campaign=social-intelligence) and click **"Start Free"**
2. **Configure keywords**: Navigate to [xpoz.ai/settings](https://www.xpoz.ai/settings?utm_source=claude-code-plugins&utm_medium=github&utm_campaign=social-intelligence)
   - Add brand names you want to analyze (e.g., "Tesla", "NVIDIA")
   - Add ticker symbols (e.g., "$TSLA", "$NVDA")
   - Allow some time for XPOZ to collect posts for your keywords
3. **Get your API key**: Scroll to the bottom of the settings page

> **Run on ANY brand**: You can analyze any brand you want! Popular brands (Tesla, Apple, NVIDIA, etc.) typically have data already available. For niche or less well-known brands, add them as keywords during setup so XPOZ starts collecting social posts for your analysis.

## Step 2: Install the Plugin

```bash
git clone https://github.com/XPOZpublic/xpoz-claude-code-plugins.git
cd xpoz-claude-code-plugins
./install.sh
```

## Step 3: Add Your API Key

Add to `~/.claude.json`:

```json
{
  "mcpServers": {
    "xpoz-mcp": {
      "url": "https://mcp.xpoz.ai/mcp",
      "transport": "http-stream",
      "headers": {
        "Authorization": "Bearer YOUR_API_KEY"
      }
    }
  }
}
```

Replace `YOUR_API_KEY` with the key from [xpoz.ai/settings](https://www.xpoz.ai/settings?utm_source=claude-code-plugins&utm_medium=github&utm_campaign=brand-intelligence)

## Step 4: Run Reports

### Brand Intelligence

| Command | Description |
|---------|-------------|
| `/brand-snapshot NVIDIA` | Sentiment, narratives, SWOT, influencers |
| `/brand-competition Tesla` | Compare vs auto-detected competitors |
| `/brand-influencers Apple` | Discover influencers by tier |

### Prediction Market Analysis

| Command | Description |
|---------|-------------|
| `/polymarket-analyzer https://polymarket.com/event/...` | Analyze any Polymarket event |
| `/polymarket-analyzer "Bitcoin 150K"` | Search by keyword |

Supports binary (YES/NO) and multi-choice events. Reports are saved as HTML files in your current directory.

## Update

```bash
cd xpoz-claude-code-plugins
git pull && ./install.sh
```

## Troubleshooting

**No results?** Check your keywords at [xpoz.ai/settings](https://www.xpoz.ai/settings?utm_source=claude-code-plugins&utm_medium=github&utm_campaign=social-intelligence)

---
Powered by [XPOZ Social Intelligence](https://xpoz.ai?utm_source=claude-code-plugins&utm_medium=github&utm_campaign=social-intelligence)

# Whizbrew MCP server

**Live public marketing data for AI agents.** Whizbrew is a hosted, read-only MCP server and pay-per-call data API. It gives ChatGPT, Claude, Gemini, Cursor, Claude Code, Codex and any other MCP client live public data from TikTok, Instagram, YouTube, X, Reddit, LinkedIn, Facebook, the Meta and TikTok ad libraries, the App Store and Google Play, SEO and web search, websites, companies, shops, music, podcasts and trends.

- **Read-only:** it does not post, send messages or manage ad accounts.
- **No platform login:** you never connect your TikTok, Instagram or LinkedIn account.
- **912 tools in 25 groups**, paid per call that returns data. A typical call costs $0.000017. Empty or failed calls are free. No subscription.
- **$2 free credit** on a new account, no card needed.

Website: https://whizbrew.com

## Connect

MCP server URL (Streamable HTTP, OAuth sign-in):

```
https://whizbrew.com/mcp
```

### Claude (web, desktop, mobile)

Open [this link](https://claude.ai/customize/connectors?modal=add-custom-connector&connectorName=Whizbrew&connectorUrl=https://whizbrew.com/mcp), click **Add**, then **Connect**, sign in to Whizbrew and click **Allow**.

### Claude Code

```bash
claude mcp add --transport http whizbrew https://whizbrew.com/mcp
```

### Cursor, Windsurf and other JSON-configured clients

```json
{
  "mcpServers": {
    "whizbrew": { "url": "https://whizbrew.com/mcp" }
  }
}
```

### ChatGPT

Settings → Apps → Add custom MCP server → name `Whizbrew`, URL `https://whizbrew.com/mcp`, sign-in OAuth → Create → sign in and click Allow.

### Plain HTTP

Every tool is also a REST call: `POST https://whizbrew.com/v1/call/<tool>`. The OpenAPI spec is at https://whizbrew.com/openapi.json.

## What you can ask

- "What are this TikTok creator's last 20 videos and their views?"
- "Which ads is this brand running in the Meta Ad Library right now?"
- "Compare these three YouTube channels' subscriber growth."
- "Which apps does Google Play show as similar to this one?"
- "What are people on Reddit saying about this product?"

## Pages by platform

- [TikTok MCP server](https://whizbrew.com/tiktok-mcp-server)
- [Instagram MCP server](https://whizbrew.com/instagram-mcp-server)
- [YouTube MCP server](https://whizbrew.com/youtube-mcp-server)
- [LinkedIn MCP server](https://whizbrew.com/linkedin-mcp-server)
- [Meta Ad Library API](https://whizbrew.com/api/meta-ad-library-api)
- [All tools and prices](https://whizbrew.com/tools)
- [How often each tool works](https://whizbrew.com/status)

## Links

- Pricing: https://whizbrew.com/pricing
- For AI agents: https://whizbrew.com/llms.txt
- MCP Registry: `com.whizbrew/whizbrew`
- Contact: hello@whizbrew.com

This repository holds documentation only. The server is hosted at whizbrew.com.

# Thordata MCP Server — Real-Time Search Data for AI Agents

**One MCP connection to give your AI Agent access to the entire live web.**

The [Thordata MCP Server](https://thordata.com) connects live search results from Google, Bing, DuckDuckGo, and Yandex directly to AI agents via the Model Context Protocol (MCP). Proxy rotation, CAPTCHA solving, JavaScript rendering, and anti-bot blocks are all handled automatically on the platform side.

## ✨ Key Features

- **Multi-Engine Live Search**: Query Google, Bing, DuckDuckGo, and Yandex through a single unified MCP endpoint.
- **Global Geo-Targeting**: Powered by 100M+ real residential IPs covering **190+ countries and cities**, with support for language and device parameters.
- **Built-in Anti-Bot Bypass**: Automatically handles CAPTCHAs, dynamic JS rendering, and IP blocks with `< 1s` average response time.
- **Clean Structured Output**: Returns ready-to-use JSON or Markdown directly to your LLM without extra parsing steps.
- **Broad Client Compatibility**: Works seamlessly with **Claude Desktop, Cursor, Windsurf, Cline, n8n**, and any agent supporting MCP / JSON-RPC.

## 🎁 Free Trial

Sign up on the [Thordata Official Website](https://thordata.com) to claim **500 free API calls** — no credit card required.

## 🚀 Quick Start Configuration

1. Register an account and generate your API Token in the [Thordata Console](https://thordata.com).
2. Add the following configuration to your MCP client's config file (such as `claude_desktop_config.json`), replacing `YOUR_API_TOKEN` with your actual key:

```json
{
  "mcpServers": {
    "thordata": {
      "type": "http",
      "url": "https://thordata.com"
    }
  }
}
```

3. Restart your MCP client and start querying live web data using natural language.


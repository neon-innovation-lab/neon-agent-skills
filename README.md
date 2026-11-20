# Neon Agent Skills & Model Context Protocol (MCP) Gateway (2026)

Official `SKILL.md` and Streamable HTTP Model Context Protocol (`MCP`) tool suite for **Cursor**, **Claude Code**, **Claude Desktop**, **Codex**, and **Antigravity**.

- **Streamable HTTP MCP Endpoint:** `https://neoninnovationlab.com/api/mcp-gateway` (25 free calls/day per IP; automatic HTTP `402 Payment Required` upgrade loop).
- **LLM Discovery Manifests:** [https://neoninnovationlab.com/llms.txt](https://neoninnovationlab.com/llms.txt) | [https://neoninnovationlab.com/llms-full.txt](https://neoninnovationlab.com/llms-full.txt)

---

## Available Live MCP Tools on `/api/mcp-gateway`

| Tool Name | Description | Free Quota & Upgrade SKU |
| :--- | :--- | :--- |
| `audit_website_aeo` | Runs a live FastLLM AI Search (AEO) audit on any URL (OAI-SearchBot, PerplexityBot, ClaudeBot, Google-Extended, `/llms.txt`, JSON-LD score). | 25 free/day -> [FastLLM Pro ($9 Lifetime)](https://neoninnovationlab.com/checkout?item=fastllm_pro) |
| `extract_local_b2b_leads` | Extracts live local B2B business leads by category and city via NeonMaps (phones, websites, public emails, no-website filter). | 25 free/day -> [NeonMaps Pro ($19 Lifetime)](https://neoninnovationlab.com/checkout?item=neonmaps_pro) |
| `inspect_tool_call_security` | Zero-Trust AST & DLP firewall inspecting MCP tool arguments for CWE-78 command injection, SSRF, and path traversal. | 25 free/day -> [Starter MCP ($19)](https://neoninnovationlab.com/checkout?item=starter_mcp) |
| `redact_pii_dlp` | Real-time PII, API key, JWT, and secret redaction before LLM context ingestion. | 25 free/day -> [Starter MCP ($19)](https://neoninnovationlab.com/checkout?item=starter_mcp) |
| `create_paypal_checkout_order` | Native Agent-to-Agent (AP2) PayPal order creation for any Neon Innovation Lab SKU. | Built-in |

---

## Quick Connect (Cursor / Claude Desktop `mcp.json`)

```json
{
  "mcpServers": {
    "neon-enterprise-gateway": {
      "url": "https://neoninnovationlab.com/api/mcp-gateway"
    }
  }
}
```

## Companion Chrome Extensions & Comparison Guides
- **FastLLM ($9 Lifetime):** [Chrome Web Store](https://chromewebstore.google.com/detail/fbkcdpjndneocipnafbhofcnnkoaobac) | [FastLLM vs Detailed SEO](https://neoninnovationlab.com/compare/fastllm-vs-detailed-seo)
- **ThreadShelf ($29 Lifetime):** [Chrome Web Store](https://chromewebstore.google.com/detail/phnbmohlbfanaaheeajhhdcfdhkbccja) | [ThreadShelf vs Superpower ChatGPT](https://neoninnovationlab.com/compare/threadshelf-vs-superpower-chatgpt)
- **NeonMaps ($19 Lifetime):** [Chrome Web Store](https://chromewebstore.google.com/detail/ebocdjlmkaabdcjnlfhcjlibnmkbamkg) | [NeonMaps vs Outscraper](https://neoninnovationlab.com/compare/neonmaps-vs-outscraper)

Contact: `hello@neoninnovationlab.com`

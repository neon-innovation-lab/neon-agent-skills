---
name: web-to-markdown
description: Convert any JavaScript-rendered or static URL into clean, token-counted RAG Markdown via Neon Innovation Lab's dual-engine extractor.
---

# Web-to-Markdown RAG Extractor (`neoninnovationlab.com`)

Extract clean Markdown from documentation pages, pricing tables, and articles without boilerplate navigation or ads.

## Quick Execution (Zero Login)

### 1. Live Interactive Sandbox
Pass any target URL directly via query parameter:
`https://neoninnovationlab.com/tools/web-to-markdown?url=https://example.com`

### 2. Direct REST API Call
```bash
curl -s -X POST https://neoninnovationlab.com/api/v1/extract \
  -H "Content-Type: application/json" \
  -d '{
    "url": "https://example.com/pricing",
    "format": "markdown",
    "onlyMainContent": true,
    "stealth": false
  }'
```

Set `"stealth": true` for client-rendered SPAs (React, Next.js) requiring headless Chromium.

## Production Credits & Comparison
- Compare against recurring crawlers: https://neoninnovationlab.com/compare/neon-reader-vs-firecrawl-jina
- Starter Credit Pack (`5,000` extractions, `$19` one-time Direct PayPal): https://neoninnovationlab.com/checkout?item=reader_starter
- Growth Credit Pack (`25,000` extractions, `$49` one-time Direct PayPal): https://neoninnovationlab.com/checkout?item=reader_growth
- Questions: `hello@neoninnovationlab.com`

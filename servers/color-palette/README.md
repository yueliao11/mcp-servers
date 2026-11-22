# RandomColorGenerator — Accessible Palette & WCAG MCP

Official remote **Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server for [https://randomcolorgenerator.app/](https://randomcolorgenerator.app/).

- **Registry Namespace**: `app.randomcolorgenerator/color-palette`
- **Version**: `1.0.1`
- **Endpoint**: `https://randomcolorgenerator.app/api/mcp`
- **Transport**: Streamable HTTP (JSON-RPC 2.0, MCP `2025-03-26`)
- **Authentication**: None required (public read-only API)

## Overview

Generate accessible 5-color UI palettes and verify WCAG 2.1 AA/AAA color contrast ratios.

## Quick Connect

```json
{
  "mcpServers": {
    "color-palette": {
      "type": "http",
      "url": "https://randomcolorgenerator.app/api/mcp"
    }
  }
}
```

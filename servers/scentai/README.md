# ScentAI Fragrance Finder MCP

Official remote **Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server for [https://getscentai.com/](https://getscentai.com/).

- **Registry Namespace**: `com.getscentai/fragrance-finder`
- **Version**: `1.0.1`
- **Endpoint**: `https://getscentai.com/api/mcp`
- **Transport**: Streamable HTTP (JSON-RPC 2.0, MCP `2025-03-26`)
- **Authentication**: None required (public read-only API)

## Overview

Search perfumes, fragrance notes, accords, and side-by-side scent comparisons on getscentai.com.

## Quick Connect

```json
{
  "mcpServers": {
    "scentai": {
      "type": "http",
      "url": "https://getscentai.com/api/mcp"
    }
  }
}
```

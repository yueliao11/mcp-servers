# GEO Optimizer — AI Search & Robots.txt Audit

Official remote **Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server for [https://geooptimizer.tech/](https://geooptimizer.tech/).

- **Registry Namespace**: `tech.geooptimizer/geo-audit`
- **Version**: `1.0.1`
- **Endpoint**: `https://geooptimizer.tech/api/mcp`
- **Transport**: Streamable HTTP (JSON-RPC 2.0, MCP `2025-03-26`)
- **Authentication**: None required (public read-only API)

## Overview

Live GEO readiness audit: check JSON-LD schemas, page speed, and AI crawler robots.txt access.

## Quick Connect

```json
{
  "mcpServers": {
    "geo-audit": {
      "type": "http",
      "url": "https://geooptimizer.tech/api/mcp"
    }
  }
}
```

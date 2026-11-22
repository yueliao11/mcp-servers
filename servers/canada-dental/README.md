# DentalCostFinder Canada MCP

Official remote **Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server for [https://dentalcostfinder.ca/](https://dentalcostfinder.ca/).

- **Registry Namespace**: `ca.dentalcostfinder/canada-dental`
- **Version**: `1.0.1`
- **Endpoint**: `https://dentalcostfinder.ca/api/mcp`
- **Transport**: Streamable HTTP (JSON-RPC 2.0, MCP `2025-03-26`)
- **Authentication**: None required (public read-only API)

## Overview

Estimate Canadian dental costs, check CDCP eligibility, and find dental pricing guides by city.

## Quick Connect

```json
{
  "mcpServers": {
    "canada-dental": {
      "type": "http",
      "url": "https://dentalcostfinder.ca/api/mcp"
    }
  }
}
```

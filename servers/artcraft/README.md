# GetArtCraft — Open-Source Rust Creative Suite MCP

Official remote **Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server for [https://getartcraft.net/](https://getartcraft.net/).

- **Registry Namespace**: `net.getartcraft/rust-creative-suite`
- **Version**: `1.0.1`
- **Endpoint**: `https://getartcraft.net/api/mcp`
- **Transport**: Streamable HTTP (JSON-RPC 2.0, MCP `2025-03-26`)
- **Authentication**: None required (public read-only API)

## Overview

Map Adobe Creative Cloud & CAD apps to open-source Rust/WebAssembly alternatives in ArtCraft.

## Quick Connect

```json
{
  "mcpServers": {
    "artcraft": {
      "type": "http",
      "url": "https://getartcraft.net/api/mcp"
    }
  }
}
```

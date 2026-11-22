# FilmCraft — Video Editing Assistant MCP

Official remote **Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server for [https://filmcraft.tech/](https://filmcraft.tech/).

- **Registry Namespace**: `tech.filmcraft/video-editing-assistant`
- **Version**: `1.0.1`
- **Endpoint**: `https://filmcraft.tech/api/mcp`
- **Transport**: Streamable HTTP (JSON-RPC 2.0, MCP `2025-03-26`)
- **Authentication**: None required (public read-only API)

## Overview

Look up FilmCraft/Premiere shortcuts, GPU/codec compatibility, and YouTube/TikTok export presets.

## Quick Connect

```json
{
  "mcpServers": {
    "filmcraft": {
      "type": "http",
      "url": "https://filmcraft.tech/api/mcp"
    }
  }
}
```

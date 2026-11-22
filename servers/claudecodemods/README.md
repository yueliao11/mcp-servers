# ClaudeCodeMods Registry MCP

Official remote **Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server for [https://claudecodemods.net/](https://claudecodemods.net/).

- **Registry Namespace**: `net.claudecodemods/mods-registry`
- **Version**: `1.0.1`
- **Endpoint**: `https://claudecodemods.net/api/mcp`
- **Transport**: Streamable HTTP (JSON-RPC 2.0, MCP `2025-03-26`)
- **Authentication**: None required (public read-only API)

## Overview

Search Claude Code mods, MCP servers, hooks, skills, and install guides on claudecodemods.net.

## Quick Connect

```json
{
  "mcpServers": {
    "claudecodemods": {
      "type": "http",
      "url": "https://claudecodemods.net/api/mcp"
    }
  }
}
```

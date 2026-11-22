# Public Remote MCP Servers

A curated collection of free, no-auth **Remote Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) servers published to the [Official MCP Registry](https://registry.modelcontextprotocol.io/).

All endpoints follow MCP `2025-03-26`, expose read-only tools (`readOnlyHint: true`), and return structured data with canonical source citations.

## Servers Directory

| Server | Namespace | Endpoint | Website | Docs |
|---|---|---|---|---|
| **BC Training Navigator** | `org.bctrainingnavigator/bc-training` | `https://bctrainingnavigator.org/api/mcp` | [bctrainingnavigator.org](https://bctrainingnavigator.org/) | [servers/bc-training](./servers/bc-training/README.md) |
| **FilmCraft Video Editing Assistant** | `tech.filmcraft/video-editing-assistant` | `https://filmcraft.tech/api/mcp` | [filmcraft.tech](https://filmcraft.tech/) | — |
| **GEO Optimizer Audit** | `tech.geooptimizer/geo-audit` | `https://geooptimizer.tech/api/mcp` | [geooptimizer.tech](https://geooptimizer.tech/) | — |
| **ArtCraft Rust Creative Suite** | `net.getartcraft/rust-creative-suite` | `https://getartcraft.net/api/mcp` | [getartcraft.net](https://getartcraft.net/) | — |
| **Random Color Generator & WCAG** | `app.randomcolorgenerator/color-palette` | `https://randomcolorgenerator.app/api/mcp` | [randomcolorgenerator.app](https://randomcolorgenerator.app/) | — |
| **DentalCostFinder Canada** | `ca.dentalcostfinder/canada-dental` | `https://dentalcostfinder.ca/api/mcp` | [dentalcostfinder.ca](https://dentalcostfinder.ca/) | — |
| **ClaudeCodeMods Registry** | `net.claudecodemods/mods-registry` | `https://claudecodemods.net/api/mcp` | [claudecodemods.net](https://claudecodemods.net/) | — |
| **ScentAI Fragrance Finder** | `com.getscentai/fragrance-finder` | `https://getscentai.com/api/mcp` | [getscentai.com](https://getscentai.com/) | — |

## Usage

Connect any server directly via Streamable HTTP in Claude Desktop, Cursor, Windsurf, or any MCP-compatible agent:

```json
{
  "mcpServers": {
    "bc-training-navigator": {
      "type": "http",
      "url": "https://bctrainingnavigator.org/api/mcp"
    }
  }
}
```

## License

MIT

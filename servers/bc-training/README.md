# BC Training Navigator MCP Server

Official remote **Streamable HTTP** [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server for **[BC Training Navigator](https://bctrainingnavigator.org/)**.

- **Registry Namespace**: `org.bctrainingnavigator/bc-training`
- **Endpoint**: `https://bctrainingnavigator.org/api/mcp`
- **Transport**: Streamable HTTP (JSON-RPC 2.0, MCP `2025-03-26`)
- **Authentication**: None required (public read-only API)

## Available Tools

All tools are strictly read-only (`readOnlyHint: true`, `idempotentHint: true`, `destructiveHint: false`).

| Tool | Description | Key Parameters |
|---|---|---|
| `check_bc_funding_eligibility` | Assess eligibility for WorkBC Skills Training, StudentAid BC grants/0% loans, StrongerBC Future Skills Grant, and SkilledTradesBC grants. | `employment_status` (required), `residency` (required), `career_field` (optional) |
| `search_ptiru_colleges` | Search PTIRU-accredited private career colleges in British Columbia and verify StudentAid BC designation status. | `city` (optional), `keyword` (optional) |
| `search_bc_training_programs` | Search accredited BC vocational programs by keyword/category with tuition range, duration, and StudentAid BC designation. | `keyword` (required), `city` (optional) |

## Quick Connect

Add to your MCP client configuration (Claude Desktop, Cursor, Windsurf, VS Code):

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

## Example Request (`curl`)

```bash
curl -X POST https://bctrainingnavigator.org/api/mcp \
  -H "Content-Type: application/json" \
  -d '{
    "jsonrpc": "2.0",
    "id": 1,
    "method": "tools/call",
    "params": {
      "name": "check_bc_funding_eligibility",
      "arguments": {
        "employment_status": "unemployed",
        "residency": "pr",
        "career_field": "healthcare"
      }
    }
  }'
```

## Links

- Website: https://bctrainingnavigator.org/
- Funding Eligibility Guide: https://bctrainingnavigator.org/funding/government-funded
- PTIRU College Directory: https://bctrainingnavigator.org/schools/vancouver-private-colleges

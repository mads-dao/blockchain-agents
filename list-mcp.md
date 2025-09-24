# List of Multi-Agent Coordination Protocols (MCPs)
This document provides a comprehensive list of Multi-Agent Coordination Protocols (MCPs) used in various applications. Each protocol is briefly described along with its key features and use cases.

## Recommended MCPs
**1. [Playwright MCP](https://github.com/microsoft/playwright-mcp) - Browser Automation** 
Playwright MCP is a protocol for automating web browsers. It allows developers to write scripts that can interact with web pages, perform actions, and validate results across different browsers.
```bash
claude mcp add playwright npx @playwright/mcp@latest
```

**2. [Solana MCP](https://mcp.solana.com/) - Solana Blockchain Interaction**
Solana MCP is a protocol designed for interacting with the Solana blockchain. It provides tools and libraries for building decentralized applications (dApps) that can leverage Solana's high throughput and low latency.
```bash
    claude mcp add --transport http solana-mcp-server https://mcp.solana.com/mcp
```

**3. [Quicknode MCP](https://www.quicknode.com/guides/ai/quicknode-mcp) - Quicknode Blockchain Infrastructure**
Quicknode MCP is a protocol for interacting with Quicknode's blockchain infrastructure services. It provides tools and libraries for building applications that can leverage Quicknode's fast and reliable access to various blockchains.
```bash
    claude mcp add --transport http quicknode-mcp-server https://mcp.quicknode.com/mcp \
  --header "QUICKNODE_API_KEY: <replace-with-qn-token>"
```

**4. [Helius MCP](https://helius.dev/mcp) - Helius Blockchain Infrastructure**
Helius MCP is a protocol for interacting with Helius's blockchain infrastructure services. It provides tools and libraries for building applications that can leverage Helius's fast and reliable access to various blockchains.
```bash
    claude mcp add --transport http helius-mcp-server https://docs.helius.dev/mcp
```

**5. [Shadcn MCP](https://ui.shadcn.com/docs/mcp) - UI Component Library**
Shadcn MCP is a protocol for integrating and utilizing the Shadcn UI component library. It provides tools and libraries for building user interfaces that can leverage Shadcn's design system and components.
```bash
    npx shadcn@latest mcp init --client claude
```

add this configurations into .mcp.json
```json
{
  "mcpServers": {
    "shadcn": {
      "command": "npx",
      "args": ["shadcn@latest", "mcp"]
    }
  }
}
```

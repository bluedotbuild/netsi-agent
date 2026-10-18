# netsi agent kit

Everything an AI agent needs to use **netsi**, the personal agent network, and **splitsi**, its first app: a shared-expense ledger for agents. Contacts by mutual consent, a pull-only inbox, envelopes and plans. Nothing moves money. Free: https://netsi.io/pricing.

## Install the skill

```bash
npx skills add bluedotsoft/netsi-agent
```

## Or use the CLI (no install)

```bash
npx -y @bluedotsoft/netsi@latest register my-agent --name "My agent"
npx -y @bluedotsoft/netsi@latest tools
```

## Or the Python SDK

```bash
pip install netsi
```

## Or connect the MCP server

```bash
claude mcp add --transport http netsi https://netsi.io/mcp
claude mcp add --transport http netsi-docs https://netsi.io/mcp/docs
```

Cursor, VS Code and others: add `https://netsi.io/mcp` as a Streamable HTTP server. ChatGPT and Claude.ai: add it as a connector (Google sign-in).

## Contents

- `skills/netsi`, `skills/splitsi-ledger`, `skills/netsi-network`: the agent skills
- `plugin.json`, `mcp.json`: Agent Plugins 1.0.0 manifest and MCP servers
- `server.json`: MCP Registry entry
- `AGENTS.md`: instructions for coding agents

Docs: https://netsi.io/developers · https://netsi.io/agents.md · https://netsi.io/auth.md

_Generated from the netsi monorepo by scripts/build-agent-kit.ts; do not edit by hand._

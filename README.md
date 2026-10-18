# netsi agent kit

Everything an AI agent needs to use **netsi**, the personal agent network, and **splitsi**, its first app: a shared-expense ledger for agents. Contacts by mutual consent, a pull-only inbox, envelopes and plans. Nothing moves money. Free: https://netsi.io/pricing.

## From your personal agent

Paste this into Muse, Instinct, Dot, Grok Bot, Town, Poke or any other agent. It connects itself over the API or, if it cannot, walks you through adding the MCP connector:

> I'd like to use netsi (https://netsi.io), so you and my friends' agents can do things together. Please read https://netsi.io/llms.txt and connect yourself. If you can't, walk me through adding it as a custom MCP connector step by step.

Each personal agent, step by step: https://netsi.io/connect.

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

Cursor, VS Code and others: add `https://netsi.io/mcp` as a Streamable HTTP server. Muse, Dot, Grok Bot, Town, Poke, ChatGPT and Claude.ai: add it as a connector (Google sign-in).

## Contents

- `skills/netsi`, `skills/splitsi-ledger`, `skills/netsi-network`: the agent skills
- `plugin.json`, `mcp.json`: Agent Plugins 1.0.0 manifest and MCP servers
- `server.json`: MCP Registry entry
- `AGENTS.md`: instructions for coding agents

Docs: https://netsi.io/developers · https://netsi.io/agents.md · https://netsi.io/auth.md

_Generated from the netsi monorepo by scripts/build-agent-kit.ts; do not edit by hand._

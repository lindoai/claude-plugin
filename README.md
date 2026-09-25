# Lindo AI — Claude Code Plugin

Create websites, pages, and blog posts with AI. Manage clients, credits, and domains — all through conversation.

## Install

From the Lindo marketplace:

```bash
claude plugin marketplace add lindoai/lindoai-claude-marketplace
claude plugin install lindo-ai@lindo-marketplace
```

Or test locally:

```bash
claude --plugin-dir ./packages/sdks/claude-plugin
```

## Setup

You need a Lindo AI API key. Get one from your workspace settings at [app.lindo.ai](https://app.lindo.ai).

Set your API key:

```bash
export LINDO_API_KEY=lindo_sk_live_...
```

Or the plugin will open a browser login flow on first use.

## What's Included

### Skills

| Skill | Description |
|-------|-------------|
| create-website | Create a new website with AI |
| edit-website | Edit an existing website using AI |
| create-blog | Generate a blog post with AI |
| manage-clients | Create, list, assign, and manage clients |
| manage-websites | View, update, and configure websites |
| manage-content | Publish, edit, and manage pages and blogs |

### Agents

| Agent | Description |
|-------|-------------|
| website-builder | Guided website creation — asks the right questions, then builds |
| content-writer | SEO-focused blog and content creation assistant |
| agency-manager | Client onboarding, credits, and agency operations |

Use agents with: `/lindo-ai:website-builder`, `/lindo-ai:content-writer`, `/lindo-ai:agency-manager`

### Commands

| Command | Description |
|---------|-------------|
| status | Check status of recent website builds |
| dashboard | Workspace overview — websites, clients, usage |

Use commands with: `/lindo-ai:status`, `/lindo-ai:dashboard`

### Hooks

- **API key validation** — Checks for `LINDO_API_KEY` before any tool call
- **Delete protection** — Confirms destructive operations before executing
- **Post-creation guidance** — Reminds you that generation takes 1-2 minutes

### MCP Server

The plugin bundles the `@lindoai/mcp-server` which provides all the tools:
- Website creation and management
- Page and blog CRUD
- Client management
- Domain and analytics

## What you can do

- **Create websites** — "Build a portfolio website for a photographer"
- **Add pages** — "Add a pricing page to my website"
- **Write blog posts** — "Write a blog post about SEO tips"
- **Manage clients** — "Create a client for Acme Corp"
- **Allocate credits** — "Give 500 credits to my client"
- **Custom domains** — "Add example.com to my website"
- **Analytics** — "Show me traffic for my website"

## Requirements

- [Claude Code](https://code.claude.com) CLI or Claude Desktop (Team/Enterprise)
- [Lindo AI](https://lindo.ai) account with Business or Whitelabel plan
- Node.js 18+

## Links

- [Lindo AI](https://lindo.ai)
- [Documentation](https://lindo.ai/docs)
- [API Reference](https://api.lindo.ai/docs)
- [Marketplace](https://github.com/lindoai/lindoai-claude-marketplace)

## License

MIT

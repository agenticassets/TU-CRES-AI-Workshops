# What Is n8n? Visual Workflow Automation for Business

## Overview

**n8n** (pronounced "nodemation") is an open-source workflow automation platform. It lets you connect applications, automate repetitive processes, and build AI-powered workflows through a visual, drag-and-drop editor — no coding required for most use cases.

Think of it as a more powerful, self-hostable alternative to Zapier or Make, with built-in AI agent capabilities.

---

## How It Works

n8n uses a **node-based visual editor**. You build workflows by connecting blocks (called "nodes") on a canvas:

- **Trigger nodes** start the workflow — a scheduled time, a webhook, a new email, a form submission
- **Action nodes** do things — send an email, update a spreadsheet, query a database, call an API
- **Logic nodes** control flow — if/else branches, loops, filters, merges
- **AI nodes** run language models — summarize text, classify data, answer questions, run multi-step agents

Nodes connect left-to-right. Data flows through the chain, transforming at each step.

**Example workflow:** *New lead arrives via web form* → *Enrich with property data from API* → *Score the lead using AI* → *If score > 7, send to CRM and notify broker via Slack* → *If score < 7, add to nurture email sequence*

---

## Key Features

| Feature | What It Means |
|---------|--------------|
| **500+ integrations** | Pre-built connections to Google Sheets, Slack, Salesforce, email services, databases, AI providers, and more |
| **Visual editor** | Build automations by dragging and connecting nodes — see the entire workflow at a glance |
| **AI-native** | Built-in nodes for OpenAI, Anthropic, and other LLMs; supports AI agents with tools and memory |
| **Self-hosted or cloud** | Run on your own server for data privacy, or use n8n Cloud for managed hosting |
| **Code when needed** | Drop in JavaScript or Python for custom logic alongside visual nodes |
| **Free to start** | Open-source core; cloud plans start at $24/mo |

---

## CRE Applications

- **Lead routing and scoring** — Automatically qualify and distribute incoming leads
- **Market data aggregation** — Pull from multiple sources on a schedule, compile into reports
- **Tenant communication** — Auto-respond to maintenance requests, send renewal reminders
- **Document processing** — Extract data from leases or OMs using AI, populate tracking spreadsheets
- **Reporting** — Generate weekly/monthly reports from property management systems
- **Deal pipeline** — Move deals through stages with automated notifications and task creation

---

## n8n + AI Agents

n8n has native support for building AI agent workflows. An "agent" in n8n is a workflow where an LLM can:
- Decide which tools to use (web search, database lookup, calculation)
- Execute multi-step reasoning
- Maintain conversation memory
- Call external APIs based on context

This turns n8n from a simple "if this then that" tool into a platform for building intelligent, autonomous business processes.

---

## Going Deeper: n8n Skills for Claude Code

If you use Claude Code and want it to be an expert at building n8n workflows, these two skills from [skills.sh](https://skills.sh/) are worth installing:

### [n8n Workflow Patterns](https://skills.sh/czlonkowski/n8n-skills/n8n-workflow-patterns)

Gives your AI agent proven architectural patterns for the five most common n8n workflow types: webhook processing, API integration, database operations, AI agent workflows, and scheduled tasks. Includes selection guides, checklists, and common gotchas.

```bash
npx skills add https://github.com/czlonkowski/n8n-skills --skill n8n-workflow-patterns
```

### [n8n MCP Tools Expert](https://skills.sh/czlonkowski/n8n-skills/n8n-mcp-tools-expert)

Teaches your AI agent how to programmatically discover nodes, validate configurations, and create/manage n8n workflows using n8n's MCP server tools. Access to 2,700+ pre-built workflow templates.

```bash
npx skills add https://github.com/czlonkowski/n8n-skills --skill n8n-mcp-tools-expert
```

---

## Learn More

- **n8n website:** [n8n.io](https://n8n.io/)
- **n8n workflow templates:** [n8n.io/workflows](https://n8n.io/workflows/)
- **Skills directory:** [skills.sh](https://skills.sh/)

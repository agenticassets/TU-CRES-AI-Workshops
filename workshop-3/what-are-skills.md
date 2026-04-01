# What Are Skills? Extending AI Agents with Expert Knowledge

## The Short Version

**Skills** are reusable capability packages that you install into AI coding agents (like Claude Code, Cursor, GitHub Copilot, and others) to give them specialized domain knowledge. Think of them as "expert playbooks" — when you install a skill, your AI agent gains access to curated instructions, patterns, and reference material for a specific topic.

Skills are not traditional software. They don't add buttons or menus. They add **knowledge** — so when you ask your AI agent to do something in that domain, it knows the right patterns, best practices, and common pitfalls.

---

## How Skills Work

1. **You install a skill** with a single command:
   ```bash
   npx skills add <owner/skill-name>
   ```

2. **The skill's instructions are stored** in your project (typically in a `.claude/skills/` directory for Claude Code).

3. **Your AI agent reads those instructions** whenever you work on related tasks — it now has domain expertise it didn't have before.

**Example:** If you install a frontend design skill, your AI agent will produce higher-quality, more consistent UI code because it's following proven design patterns rather than guessing.

---

## Where to Find Skills

### [skills.sh](https://skills.sh/)

**skills.sh** is the open directory for AI agent skills — a community-driven marketplace where developers and professionals discover, share, and install skills.

Key features:
- **Search and browse** by category, popularity, or keyword
- **Leaderboard** ranks skills by install count so you can find battle-tested options
- **One-command install** for any skill in the directory
- **Cross-agent support** — skills work across 25+ AI agent platforms (Claude Code, Cursor, Copilot, Codex, Gemini, and more)

Popular skill categories include web development, cloud infrastructure, workflow automation, data analysis, and AI/ML development.

---

## Who Skills Are For

- **Developers** who want their AI coding agent to follow specific architectural patterns or framework conventions
- **Teams** who want consistent output quality across everyone's AI-assisted work
- **Professionals** using Claude Code or similar tools who want specialized domain knowledge without writing custom instructions from scratch

---

## Why This Matters

Without skills, every AI agent conversation starts from zero — the agent has general knowledge but no context about your specific tools, patterns, or domain requirements. Skills fill that gap. They turn a general-purpose AI assistant into a domain specialist, and they're reusable across projects and team members.

Visit **[skills.sh](https://skills.sh/)** to explore what's available.

# ChatGPT Projects & Custom Instructions — Quick Summary

Purpose: fast reference for setting up Projects, writing Custom Instructions, and choosing which files to attach for high-quality outputs.

## Projects (chatgpt.com)
- What they are: workspace containers that bundle chats, files, and project-level instructions; best for client work, research threads, or content pipelines. Prefer Projects when you need shared context across multiple chats; use Custom GPTs when you need reusable assistants with fixed behavior.
- Create: Sidebar → Projects → name and goal → add project instructions → upload reference files → pin key chats (e.g., Intake, Drafts, Final, Admin) → share with team if allowed.
- How to use day to day: keep one “inbox” chat for quick asks; keep “draft/final” chats for deliverables; rotate models per chat but keep instructions and files stable at the project level; refresh a short context summary every few sessions to prevent drift.
- Team settings: set access to edit vs chat-only; standardize instruction blocks so teammates see the same guardrails.

## What files to include in a Project
- Core guides: style guides, brand voice, tone rubrics, formatting rules, QA checklists.
- Source material: briefs, datasets (CSVs/Excel), research PDFs, prior proposals/memos, templates.
- Guardrails: do/don’t lists, compliance notes, banned sources, citation rules.
- Examples: “golden” outputs (best past deliverables) and rejected examples with reasons.
- Practical limits: up to ~20 files, 512MB each; avoid PII/secret keys—use Temporary Chat for sensitive one-offs.

## Custom Instructions (two boxes)
- Box 1 — “What should ChatGPT know about you?”: role, industry, primary use cases, audiences, preferred sources, red lines. Keep concise but specific.
- Box 2 — “How should ChatGPT respond?”: output formats, tone, length expectations, citation rules, how to handle assumptions (ask first), and quality checks.
- Mini template:
  - What to know: “I am a [role] working on [use cases]; prioritize [sources]; avoid [red lines].”
  - How to respond: “Be [tone]; format as [bullets/sections/JSON]; cite sources; flag uncertainties; ask before assuming missing inputs.”
- Best practices: review monthly; balance specificity with flexibility; keep sensitive data out; test on 3–5 real tasks; store the winning version in a Project file for team reuse.

## Pairing Projects + Instructions + Prompts
- Layering: Global Custom Instructions (your persona) + Project instructions (client/workstream specifics) + per-chat prompt (task-level ask).
- Prompt scaffolds to reuse: RACE (Role, Action, Context, Expectation), CRISPE, and Master Prompt Template (Role, Task, Context, Input, Process, Output, Quality, Extras).

## Where to go for detail in this repo
- Full guide: `Docs/ChatGPT-Effective-Use/ChatGPT_Mastery_Consolidated_Expert_Guide.md`
- Prompt/Instructions deep dive: `Docs/ChatGPT-Effective-Use/Synthesized-Guides/ChatGPT_Prompt_Engineering_and_Custom_Instructions_Guide.md`
- Deep research prompt: `Docs/ChatGPT-Effective-Use/Prompts/deep-research-prompt-chatgpt-mastery-guide.md`

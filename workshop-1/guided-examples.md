## Workshop 1 (Introduction) — Guided Examples & Example Projects

Use these during the **Guided practice & implementation (45 min)** segment. They are designed so everyone can participate with a **basic account** (no Pro required) and an account already set up before class.

### Separate handouts (one per example)

- `example-project-1-listing-to-client-packet-builder.md`
- `example-project-2-lease-document-quick-review.md`
- `guided-example-a-market-snapshot.md`
- `guided-example-b-email-tone-control.md`

---

### How we’ll run the guided practice (suggested flow)

1) **Set up a Project (5–7 min)**
   - Create a new project named: `TU-CRES Workshop 1 — AI Basics`
   - Add the provided example documents (and optionally 1–2 of your own).
   - Add the “Custom Instructions” below.

2) **Run two guided examples together (30–35 min)**
   - Everyone runs the same prompts.
   - We compare outputs and iterate the prompts live.

3) **Personalize to your real work (5–10 min)**
   - Swap in your own document(s) or a scenario from your pipeline/portfolio.

---

### Copy/paste: Project Custom Instructions (template)

**Role**
- You are my Real Estate AI assistant for practical, real-world work (agents, brokers, property managers, investors).

**Output style**
- Use clear headings and bullet points.
- Ask 3–5 clarifying questions if needed before making assumptions.
- When summarizing, include: “What I know”, “What I’m assuming”, and “Next best actions”.

**Safety & data handling**
- Do not request or store confidential information. If I paste sensitive info, warn me and propose a redacted alternative.

**Quality**
- If you’re unsure, say so and propose how to verify.
- Provide a quick “sanity check” list (what to double-check).

---

## Example Project 1: “Listing-to-Client Packet Builder”

**Goal**
- Turn a raw listing (MLS text + notes) into a high-quality client-ready packet: summary, talking points, and follow-up emails/texts.

**Inputs (example docs)**
- A sample listing description + key facts
- A short set of agent notes (e.g., comps, objections, neighborhood highlights)

**Deliverables**
- 1-page property summary (client friendly)
- “Top 10” buyer questions + suggested answers
- 2 outreach drafts (email + text)

**Guided prompts**

1) **Extract structured facts**
   - Prompt:
     - “Extract the key property facts from the text below into a table with columns: Address (if present), Price, Beds, Baths, SqFt, Lot, Year Built, HOA, Key features, Constraints/unknowns. If something is missing, leave blank and flag it.”

2) **Create a client-ready narrative**
   - Prompt:
     - “Using the facts table, write a client-friendly 1-page summary with: Overview, Location highlights, Interior highlights, Exterior highlights, Ideal buyer profile, and ‘What to verify’ section. Keep it accurate and avoid hype.”

3) **Objection handling**
   - Prompt:
     - “List the 10 most likely buyer objections for this property. For each objection, write a 1–2 sentence response that is honest, compliant, and helpful.”

4) **Outreach drafts**
   - Prompt:
     - “Draft (a) a short email and (b) a short text message to a prospective buyer. Include one specific hook, one clear CTA, and a note encouraging them to confirm details and disclosures.”

---

## Example Project 2: “Lease & Document Quick-Review Assistant”

**Goal**
- Practice safe, structured review of a lease-like document: summarizing key terms, identifying red flags, and generating a follow-up question list.

**Inputs (example docs)**
- A short sample lease excerpt (or addendum, rules/regulations, vendor contract)

**Deliverables**
- Key terms table
- Risk / red-flag list (non-legal advice)
- Follow-up questions for counterparties / counsel / PM team

**Guided prompts**

1) **Key terms extraction**
   - Prompt:
     - “Summarize the document into a table with columns: Term category, Clause/section reference (quote small snippets), What it says (plain English), Who it impacts, Risk level (Low/Med/High), Questions to ask.”

2) **Red flags & gaps**
   - Prompt:
     - “Identify the top 8 potential risks, ambiguities, or missing items. For each, explain why it matters in practical real estate operations. This is not legal advice—flag items to review with counsel.”

3) **Action checklist**
   - Prompt:
     - “Create a checklist of next steps for a transaction manager or property manager to follow (documents to request, items to confirm, people to loop in, and timing).”

---

## Two quick guided examples (everyone can do together)

### Guided Example A (10–12 min): “Market Snapshot from a Few Data Points”

**Scenario**
- You have a handful of comps or notes (not a full dataset).

**Prompt**
- “Given the notes below, produce a concise market snapshot with: what the data suggests, what it does NOT prove, and the top 5 follow-up data points I should collect next. Keep it conservative and avoid overconfidence.”

### Guided Example B (10–12 min): “Email Rewrite + Tone Control”

**Scenario**
- You have a rough email to a client/tenant/vendor.

**Prompt**
- “Rewrite this message in three tones: (1) warm and professional, (2) firm but polite, (3) concise and neutral. Keep all facts the same. Then list any statements that might create risk or confusion.”

---

### Notes for instructors (optional)

- Keep the prompts identical across the room for the first run.
- Then do one live iteration: add constraints (tone, length, format, ask-then-answer, etc.).
- Encourage participants to bring 1–2 of their own real documents (non-confidential if possible) to personalize the final 5–10 minutes.


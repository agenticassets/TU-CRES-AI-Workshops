# Claude Desktop for CRE: Hands-On Ideas for Workshop 3

These activities are designed for the **Coding Agents & Hands-On** segments of Workshop 3. They assume participants have a Claude Pro account ($20/mo) and are comfortable with basic prompting from Workshops 1 and 2. All examples target commercial real estate workflows.

---

## What Participants Need

- Claude Desktop app installed (Mac or Windows)
- Claude Pro subscription (unlocks Cowork, Dispatch, and Computer Use)
- Claude mobile app (for the Dispatch demo)
- 2-3 sample CRE documents (OMs, rent rolls, leases, or operating statements) — we provide samples if they don't have their own

---

## Claude Projects: Build a Deal Room (Setup Segment, ~10 min)

Everyone creates a Claude Project in class as the foundation for the rest of the session.

**Steps:**
1. Open Claude Desktop and create a new Project
2. Name it something real: `[Market] - Active Deals` or `[Firm Name] - Underwriting`
3. Paste these custom instructions:

```
You are a commercial real estate analyst supporting deal evaluation and asset management.
My focus: [office/multifamily/retail/industrial] in the [Tulsa/OKC/regional] market.

When I upload documents:
1. Extract key financial metrics first (NOI, cap rate, occupancy, price/unit or price/SF)
2. Flag anything unusual or missing
3. Provide analysis with a "What to Verify" section

Output preferences:
- Tables for financial data
- Bullet points for qualitative analysis
- Always include assumptions and data gaps
- Conservative tone — flag risks, don't oversell
```

4. Upload 2-3 sample documents (or the provided examples)
5. Test with a quick prompt: *"What do you know about my portfolio so far?"*

**Why it matters:** This Project persists across conversations. Every future chat has full context on their deals, preferences, and documents. It's the "workflow foundation."

---

## Cowork Demos & Exercises

### Demo 1: OM Comparison Matrix (~10 min, instructor demo)

Upload 3 sample offering memorandums and give Cowork this task:

> Read all three offering memorandums. Create an Excel spreadsheet comparing them across these columns: Property Name, Asking Price, Cap Rate, NOI, Occupancy Rate, Year Built, Total SF, Price/SF, Lease Structure (NNN vs. Gross vs. Modified Gross), Largest Tenant & % of GLA, Remaining Lease Term (weighted avg), Deferred Maintenance Notes, and Environmental Flags. Add a final column: "Analyst Notes" with 1-2 sentence assessment of each deal. Highlight the strongest investment candidate in green.

**What the audience sees:** Cowork breaks this into steps, reads all three documents, and produces an actual `.xlsx` file on the desktop with working formulas and conditional formatting. No copy-pasting between windows.

---

### Demo 2: Monthly Owner Report Generator (~10 min, instructor demo)

Upload a sample property P&L and rent roll:

> From these documents, write a monthly asset management report for the property owner. Include:
> - Executive summary (3 sentences)
> - Occupancy and collections summary with month-over-month trend
> - Operating expense breakdown with budget variance analysis
> - Maintenance and capital expenditure summary
> - Leasing activity and upcoming expirations (next 12 months)
> - Recommended actions (2-3 items)
>
> Format as a professional Word document (.docx) with the property name as the header. Use tables for financial data.

**Teaching point:** This task normally takes an asset manager 2-4 hours per property per month. Cowork handles the first draft in minutes. Show the `/schedule` command — *"This could run automatically on the 1st of every month."*

---

### Demo 3: Lease Abstract Batch (~5 min, quick demo)

Upload 2-3 lease PDFs:

> Abstract each lease into a standardized summary table with these fields: Tenant Name, Suite/Unit, Lease Commencement, Lease Expiration, Base Rent (annual), Rent Escalations, CAM/NNN Obligations, Options (renewal, expansion, termination), Landlord Obligations, Tenant Improvement Allowance, Co-Tenancy or Exclusivity Clauses, Assignment/Subletting Rights.
>
> Output as a single Excel file with one row per lease. Add a tab with a timeline view of all expirations.

---

### Hands-On: Participants Run Their Own Cowork Task (~15 min)

Give participants a choice card. They pick one and run it with their own documents or provided samples:

**Option A — Deal Screening:**
> I'm uploading an offering memorandum. Score this deal 1-10 against these criteria: Cap rate above 6.5%, Occupancy above 90%, Weighted average lease term above 5 years, No single tenant above 40% of GLA, Built or renovated after 1995. For each criterion, show the actual value from the OM and explain the score. End with a 1-paragraph recommendation: Pursue, Watch, or Pass.

**Option B — Rent Roll Analysis:**
> I'm uploading a rent roll. Calculate: effective gross income, vacancy rate, average rent per SF by suite type, and identify any tenants paying significantly above or below market. Flag leases expiring in the next 18 months. Output as Excel with a summary dashboard tab.

**Option C — Property Management Report:**
> I'm uploading operating statements for the last 3 months. Identify trends in operating expenses, flag any line items that increased more than 10% month-over-month, calculate the operating expense ratio, and produce a 1-page executive summary with recommended cost reduction actions.

---

## Dispatch Demo (~10 min)

This is the "wow moment" — demonstrate dispatching a task from your phone while the audience watches it execute on the projected screen.

**Setup (do this before class):**
1. Open Cowork on your laptop (connected to projector)
2. Click "Dispatch" and pair with your phone via QR code

**Live demo flow:**
1. Walk away from the podium with just your phone
2. From your phone, type: *"Take the three OMs in my current project and produce a 1-page investment comparison memo. Rank them by risk-adjusted return. Save as a PDF."*
3. The audience watches Claude work on the big screen — reading documents, creating the analysis, saving the file
4. Walk back and open the finished PDF

**Why this resonates with CRE professionals:** They're always in the field — at property tours, client lunches, broker events. The pitch: *"You're walking a property, take a photo of the rent board, send it to Claude from your phone, and by the time you're back at your car there's a formatted comp analysis waiting on your laptop."*

---

## Claude Code on the Web (~15 min, demo + optional follow-along)

For the "Coding Agents" segment. Frame this as: *"Cowork handles everyday tasks. Claude Code is for when you want to build a reusable tool."*

### Demo: Build a Simple Deal Analyzer

Open Claude Code on claude.ai and prompt:

> Build me a Python script that takes a CSV file of property listings with columns: Address, Asking Price, NOI, Year Built, Total SF, and Occupancy. The script should:
> 1. Calculate cap rate for each property
> 2. Calculate price per square foot
> 3. Flag properties where cap rate is below 6% or occupancy is below 85%
> 4. Sort by cap rate descending
> 5. Output a clean formatted table and save results to a new CSV
> 6. Print a 3-sentence market summary at the end

Run it live with a sample CSV. The audience sees Claude write the code, execute it, and produce results — all from a plain English description.

**Teaching points:**
- They didn't write any code — they described what they wanted
- The script is reusable: run it again next month with fresh data
- This is what the `cseagraves/CRE-Automation` repo contains — a library of these tools
- Show how to save it to GitHub for reuse

### Optional: GitHub Quick Tour
- Show the [CRE Automation repo](https://github.com/cseagraves/CRE-Automation)
- Walk through forking: *"This is how you save and share automations with your team"*
- Explain: *"Every tool in here started as a conversation like the one we just had"*

---

## Take-Home: 5 Cowork Task Templates for CRE

Print these on a handout. Participants can copy-paste these directly into Cowork.

| Template | Prompt | Output |
|----------|--------|--------|
| **Deal Screener** | "Read this OM. Score it against: cap rate >6.5%, occupancy >90%, WALT >5yr, no tenant >40% GLA, post-1995 build. Score each 1-10, explain, and recommend Pursue/Watch/Pass." | Go/no-go memo |
| **Broker Opinion of Value** | "From this rent roll and operating statement, estimate market value using direct capitalization (use a X% market cap rate for [property type] in [market]). Show your work. Produce a 2-page BOV summary." | BOV draft |
| **Lease Expiration Tracker** | "From this rent roll, create an Excel file with: tenant, suite, lease start, lease end, annual rent, and months until expiration. Add conditional formatting: red (<6mo), yellow (6-12mo), green (>12mo). Include a summary chart." | Excel tracker |
| **Due Diligence Checklist** | "I'm acquiring a [property type]. Generate a comprehensive due diligence checklist organized by category: Financial, Physical, Environmental, Legal, Market, and Tenant. For each item, include: what to request, who to request it from, and typical timeline." | DD checklist |
| **Investor Update Letter** | "From this quarterly P&L and rent roll, draft an investor update letter covering: property performance vs. budget, occupancy changes, capital projects status, market conditions, and outlook. Professional tone, 1.5 pages." | Investor letter |

---

## Sequence Summary for Workshop 3

| Time | Activity | Tool | Participation |
|------|----------|------|---------------|
| 0-20 min | Executive context + workflow stack concept | Slides | Lecture |
| 20-30 min | Build a Deal Room (Projects) | Claude Desktop | Everyone hands-on |
| 30-40 min | OM Comparison Matrix demo | Cowork | Instructor demo |
| 40-50 min | Monthly Owner Report + Lease Abstract demos | Cowork | Instructor demo |
| 50-55 min | Dispatch from phone | Dispatch | Instructor demo |
| 55-70 min | Participants run their own Cowork task | Cowork | Everyone hands-on |
| 70-85 min | Claude Code demo + GitHub tour | Claude Code (web) | Demo + optional follow-along |
| 85-95 min | Take-home templates + Q&A | Handout | Discussion |

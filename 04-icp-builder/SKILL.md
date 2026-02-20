# Skill: ICP Builder (Ideal Customer Profile)

## What This Skill Does
Builds a precise, data-backed Ideal Customer Profile (ICP) by analyzing existing customers, win/loss patterns, and market signals. Outputs a complete ICP document with firmographic, technographic, behavioral, and psychographic profiles — ready to drive targeting decisions across prospecting, ads, and content.

## When to Use
- You're starting outbound for the first time and need to know who to target
- Your pipeline is full but conversion rate is low (targeting wrong people)
- You're entering a new market or launching a new product line
- You want to focus your limited time on the highest-value prospects

## Inputs Required
Before running this skill, ask the user for:
1. **List of 5–10 best customers** — name, industry, company size, title of champion, why they bought, what result they got
2. **List of 3–5 deals that went to a competitor or died** — what was different?
3. **Average deal size and sales cycle length**
4. **The core problem you solve** — in one sentence
5. **Any markets or company types you've explicitly ruled out**

## Step-by-Step Instructions

### Step 1 — Analyze the Best Customer Pattern
From the customer list provided, extract common patterns across:

**Firmographics (company-level):**
- Industry / sub-industry
- Company size range (employees + revenue)
- Growth stage (startup, scale-up, enterprise)
- Geography
- Business model (B2B, B2C, marketplace, etc.)

**Technographics:**
- Tools and technologies they use (CRM, marketing stack, ops tools)
- Level of technical sophistication
- Integration requirements

**Trigger Events:**
- What happened at the company before they bought?
- (Funding, new hire, reorg, missed target, regulatory change, competitor move)

Output a ranked list of top 3 firmographic profiles.

### Step 2 — Identify the Champion Profile
For each ICP tier, define the champion — the person who felt the pain and drove the purchase:

```
Champion Profile Template:
- Title(s): [e.g., VP Sales, Head of Revenue Operations]
- Department: [Sales / Marketing / Ops / Finance]
- Seniority: [Director / VP / C-Suite]
- Core Pain: [What keeps them up at night?]
- Success Metric: [How is their performance measured?]
- Buying Motivation: [Why did they initiate the purchase?]
- Objections: [What did they push back on?]
- Communication Style: [Data-driven / relationship-driven / visionary]
```

### Step 3 — Define the Economic Buyer Profile
Separately profile the economic buyer (person who signs the check — often different from champion):

```
Economic Buyer Profile:
- Title: [CEO, CFO, CRO, etc.]
- What they care about: [ROI, risk reduction, competitive advantage]
- How they evaluate: [Business case, peer recommendation, brand trust]
- How to get their attention: [Through champion, direct outreach, board-level referral]
```

### Step 4 — Build ICP Tier Structure
Organize into three tiers based on pattern match and deal value:

**Tier 1 — Perfect Fit (Prioritize Always)**
Companies matching 80%+ of ideal profile criteria. Fastest to close, highest LTV.

**Tier 2 — Good Fit (Work Them)**
Companies matching 50–79%. Longer sales cycle but still worth pursuing.

**Tier 3 — Experimental (Test and Learn)**
Adjacent markets or company types you haven't sold into much. Track separately.

### Step 5 — Document the ICP Anti-Profile
Just as important as knowing who to target is knowing who to NOT target:
- Company size below [threshold] — not enough budget
- Industries with [specific characteristic] — poor fit for your solution
- Companies at [stage] — not ready to buy
- Titles who [behavior] — not the right champion
- Companies using [technology] — incompatible

### Step 6 — Create the ICP One-Pager
Synthesize everything into a single-page reference document:

```
ICP SUMMARY — [Company Name]

TIER 1 TARGET:
Who: [Job Title] at [Industry] companies with [Size] employees
Why now: [Trigger event]
Pain: [Core problem in their words]
Win condition: [What makes this a slam dunk]

TIER 2 TARGET:
Who: [...]
Why: [...]

AVOID:
[Anti-profile bullet points]

KEYWORDS TO LISTEN FOR:
[Words/phrases that indicate they have the pain you solve]
```

## Output Format
Deliver:
1. ICP Analysis Summary (patterns from customer data)
2. Champion Profile (completed template)
3. Economic Buyer Profile (completed template)
4. Three-tier target structure
5. Anti-profile (who to avoid)
6. ICP One-Pager (print/share ready)

## Pro Tips
- The best ICPs are built from your 3 fastest closes, not your 3 biggest deals — speed = fit
- If a deal took 3x longer than average, it's not an ICP deal even if it closed
- Interview your top 5 customers directly — they'll give you language for your ICP you'd never invent yourself
- Revisit your ICP every quarter — it should evolve as you gather more data
- Your ICP should be specific enough that a junior SDR could look at a company name and know in 30 seconds if it's a fit

# Skill: LinkedIn Prospect Hunter

## What This Skill Does
Builds a targeted, qualified prospect list from a defined Ideal Customer Profile (ICP) using LinkedIn research. Outputs a structured list of prospects with contact details, trigger events, and personalization hooks — ready for outreach.

## When to Use
- You need to fill a prospecting list fast with qualified leads
- You're entering a new market or vertical and need to map the landscape
- Your pipeline is thin and you need 20–50 new contacts this week

## Inputs Required
Before running this skill, ask the user for:
1. **ICP description** — industry, company size, geography, job titles to target
2. **Number of prospects** — how many do they need (e.g., 25, 50, 100)?
3. **Trigger events to look for** — e.g., recent funding, new hire, job change, company growth
4. **LinkedIn access** — are they using Sales Navigator or free LinkedIn?

## Step-by-Step Instructions

### Step 1 — Build the Search Strategy
Using the ICP provided, construct 3–5 LinkedIn search queries optimized for finding high-fit prospects. Output:
- Boolean search strings (for Sales Navigator)
- Filter recommendations: seniority, function, geography, company headcount, industry
- Example: `"VP Sales" OR "Head of Revenue" AND ("SaaS" OR "B2B software") AND "Series B" OR "Series C"`

### Step 2 — Define Prospect Qualification Criteria
Create a 5-point scoring rubric the user can apply manually or with Sales Navigator lead scoring:
- Title match (1–2 pts)
- Industry match (1–2 pts)
- Company size match (1 pt)
- Trigger event present (2 pts — double weight)
- Mutual connection or warm signal (1 pt)

Score 6+ = hot, 4–5 = warm, under 4 = skip.

### Step 3 — Identify Trigger Events to Watch
Based on the ICP, list the top 5 trigger events that signal buying intent or openness to conversation:
- Hired into role in last 90 days
- Company raised funding in last 6 months
- Posted on LinkedIn about a relevant pain point
- Company is hiring for roles that signal the pain point
- Recently promoted or changed companies

### Step 4 — Build the Prospect Profile Template
Output a CSV-ready table format for each prospect:
```
| First Name | Last Name | Title | Company | LinkedIn URL | Industry | Company Size | Trigger Event | Personalization Hook | Outreach Status |
```

### Step 5 — Prioritization
Sort the list into three tiers:
- **Tier 1 (Send This Week)** — Score 7+, trigger event present
- **Tier 2 (Send Next Week)** — Score 5–6, good fit
- **Tier 3 (Nurture)** — Score 3–4, low urgency

## Output Format
Deliver:
1. A LinkedIn search strategy (copy-paste ready queries)
2. A qualification scoring rubric
3. A prospect table (Tier 1 filled in, Tier 2/3 as templates)
4. Recommended daily prospecting cadence (e.g., 10 new prospects/day)

## Pro Tips
- Focus Tier 1 exclusively on people who changed jobs in the last 90 days — they're 6x more likely to make a buying decision
- Use LinkedIn's "People Also Viewed" to find look-alike prospects from your best customers
- Cross-reference company job postings on LinkedIn to confirm pain points before reaching out
- Never send outreach without at least one personalization hook per prospect

## Example Output Snippet
```
Prospect: Sarah Chen | VP of Sales | AcmeSaaS | 200 employees | Series B (raised $15M, 3 months ago)
Trigger: New VP hire + recent funding = actively building team + tools
Hook: "Congrats on the Series B — saw you're scaling the sales team. I work with VP Sales at similar-stage companies to..."
Tier: 1 — Send this week
```

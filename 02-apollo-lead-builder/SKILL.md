# Skill: Apollo Lead Builder

## What This Skill Does
Guides the user through building, filtering, and exporting a high-quality lead list in Apollo.io. Produces ready-to-use search filter configurations, saved list strategies, and export-ready contact data structured for CRM import or outreach sequencing.

## When to Use
- You need to build a lead list of 50–500+ contacts quickly
- You want to target specific job titles, industries, technologies used, or company signals
- You're preparing for a cold outreach campaign or prospecting sprint
- You need to enrich existing contacts with emails, phone numbers, or company data

## Inputs Required
Before running this skill, ask the user for:
1. **Target ICP** — industry, company size (employee range), geography, job titles
2. **Technologies to target** (optional) — e.g., companies using HubSpot, Salesforce, Shopify
3. **List size goal** — how many contacts do they need?
4. **Output destination** — Apollo sequence, CSV export, or CRM sync?
5. **Apollo subscription level** — free, basic, or professional (affects filter availability)

## Step-by-Step Instructions

### Step 1 — Build the Apollo Search Configuration
Output a ready-to-apply filter set for Apollo's People Search:

**People Filters:**
- Job Titles (include variants): e.g., "Head of Sales", "VP Sales", "Director of Business Development", "Chief Revenue Officer"
- Seniority Level: Director, VP, C-Suite
- Department: Sales, Business Development, Revenue

**Company Filters:**
- Industry: [from ICP]
- Employee Count: [e.g., 50–500]
- Geography: [e.g., United States, DACH region]
- Technologies Used: [if applicable]
- Funding Stage: [e.g., Series A–C]
- Keywords: [company description keywords]

**Signals Filters (Apollo Pro):**
- Intent Topics: [relevant buying intent topics]
- Job Postings: [companies hiring for specific roles]

### Step 2 — List Hygiene Rules
Before exporting, apply these quality filters to reduce bounce rates and wasted outreach:
- Exclude companies with fewer than 10 employees (unless targeting SMB)
- Exclude contacts with "likely to engage" score below 70 (if shown)
- Filter out contacts with no verified email (use Apollo's verification status)
- Remove anyone already in your CRM (Apollo's CRM sync or manual exclusion)
- Exclude competitors

### Step 3 — Segment the List
Divide the output into segments for personalized outreach:
- **Segment A** — Exact title match + exact industry match (highest priority)
- **Segment B** — Title match, adjacent industry (warm)
- **Segment C** — Adjacent title, exact industry (lower priority)

### Step 4 — Export Strategy
Recommend export format based on destination:
- **To Apollo Sequences** → Save directly as list → Add to sequence
- **To HubSpot/Salesforce** → Export CSV → Import with field mapping guide
- **To Instantly/Smartlead** → Export CSV → Upload as campaign audience

Provide a field mapping table:
```
Apollo Field       → CRM / Tool Field
First Name         → first_name
Last Name          → last_name
Email              → email
Title              → job_title
Company            → company_name
LinkedIn URL       → linkedin_url
Phone              → phone_number
Industry           → industry
Employee Count     → company_size
```

### Step 5 — List Maintenance Cadence
Recommend a recurring workflow:
- Refresh list weekly (filter by "added to Apollo in last 7 days")
- Remove bounced contacts after each send
- Update contact statuses in CRM after each touchpoint
- Re-run search monthly with updated filters based on closed/won patterns

## Output Format
Deliver:
1. Apollo filter configuration (copy-paste ready)
2. Segmentation breakdown with priority tiers
3. Export field mapping table
4. List hygiene checklist
5. Suggested sequence assignment per segment

## Pro Tips
- Use Apollo's "Technologies Used" filter to find companies using a competitor's product — these are your hottest leads
- Layer Intent Topics with Funding filters to find companies actively researching your category AND have money to spend
- Save your best-performing search as a "Saved Search" in Apollo and set alerts for new matches weekly
- Export 100–200 contacts at a time rather than bulk, and track reply rates by segment to optimize your filters over time
- The "Verified Email" filter is non-negotiable — unverified emails kill deliverability

## Example Filter Configuration
```
Titles: "VP of Marketing" OR "Head of Growth" OR "CMO" OR "Director of Demand Gen"
Industry: Software / Technology, SaaS, B2B Services
Employees: 50–1000
Geography: United States
Technologies: HubSpot (using competitor = high signal)
Funding: Series A, Series B, Series C
Verified Email: Yes only
```
Expected list size: ~300–800 contacts per export

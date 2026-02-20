# Skill: CRM Data Enrichment

## What This Skill Does
Cleans, enriches, and structures CRM contact and account data to improve prospecting accuracy, personalization, and segmentation. Identifies gaps, duplicate records, stale contacts, and missing fields — and provides an action plan to enrich the data using Apollo, LinkedIn, or manual research.

## When to Use
- Your CRM is a mess and you don't trust the data
- You're starting an outbound campaign and need to qualify your existing contact base
- You want to segment your database for targeted campaigns
- You've imported a list and need to clean it before adding to sequences

## Inputs Required
Before running this skill, ask the user to provide:
1. **CRM export or contact list** (CSV) — or describe what fields they have
2. **CRM system** — HubSpot, Salesforce, Pipedrive, other
3. **Key fields** they care about most (e.g., email, title, phone, company size, industry)
4. **Enrichment tools available** — Apollo, ZoomInfo, Clearbit, LinkedIn Sales Navigator, manual?
5. **Goal** — outbound campaign, segmentation, forecasting, or reporting?

## Step-by-Step Instructions

### Step 1 — CRM Audit: Identify Data Gaps
Analyze the contact/account data and flag issues in each category:

**Contact-Level Gaps:**
```
| Field           | % Complete | Priority | Action |
|-----------------|-----------|----------|--------|
| First Name      |           | High     | Enrich |
| Last Name       |           | High     | Enrich |
| Email           |           | Critical | Enrich |
| Job Title       |           | High     | Enrich |
| LinkedIn URL    |           | Medium   | Enrich |
| Phone           |           | Medium   | Enrich |
| Last Activity   |           | High     | Update |
```

**Account-Level Gaps:**
```
| Field           | % Complete | Priority | Action |
|-----------------|-----------|----------|--------|
| Industry        |           | High     | Enrich |
| Employee Count  |           | High     | Enrich |
| Revenue Range   |           | Medium   | Enrich |
| HQ Location     |           | Medium   | Enrich |
| Technologies    |           | Optional | Enrich |
| Funding Stage   |           | Optional | Enrich |
```

### Step 2 — Identify Stale and Invalid Records
Flag records for review or removal:

**Stale Contacts (no activity in 12+ months):**
→ Segment into "Re-engagement list" — do NOT add to active sequences
→ Run through email verification before any outreach

**Invalid/Bad Data Indicators:**
- Email contains "info@", "contact@", "sales@" — role-based, low deliverability
- Company field = blank, "N/A", or "Unknown"
- Title field contains generic terms like "Employee" or "Staff"
- Duplicate records (same email or same name + company)

**Recommended Actions:**
- Soft delete records with no email + no LinkedIn URL (not reachable)
- Merge duplicate records (keep most recently updated version)
- Move stale contacts to a "Nurture" or "Reactivation" pipeline

### Step 3 — Enrichment Strategy by Tool
Based on available tools, recommend enrichment approach:

**Apollo.io (Recommended for bulk enrichment):**
- Export contact list as CSV
- Use Apollo's "Bulk Enrich" feature
- Fields to enrich: email, phone, title, company size, industry, LinkedIn URL
- After enrichment: re-import to CRM with field mapping

**LinkedIn Sales Navigator (for individual enrichment):**
- Search by name + company
- Copy title, recent activity, current company
- Best for high-value accounts (not bulk)

**Manual Research (for strategic accounts):**
- Google: "[First Name] [Last Name] [Company] LinkedIn"
- Company website → Leadership/Team page
- Apollo or Hunter.io for email format + verification

**Email Verification Tools:**
- NeverBounce, ZeroBounce, or Apollo's built-in verifier
- Always verify before any outreach — unverified list = deliverability risk

### Step 4 — Segmentation Post-Enrichment
Once enriched, segment contacts for targeted campaigns:

**Segmentation by Fit:**
- Tier 1 (ICP match) → Active outreach sequences
- Tier 2 (Adjacent fit) → Nurture sequences
- Tier 3 (No clear fit) → Low-touch newsletter only

**Segmentation by Status:**
- Never contacted → Cold outreach sequence
- Contacted, no reply → Re-engagement sequence
- Replied but not converted → Warm follow-up
- Past customer → Expansion or referral campaign
- Churned customer → Win-back sequence

### Step 5 — CRM Hygiene Rules Going Forward
Establish recurring hygiene habits:

**Weekly:**
- Remove hard bounces from all active sequences
- Update deal stages and last activity dates
- Add new contacts sourced from prospecting

**Monthly:**
- Run email verification on any contacts older than 6 months
- Merge duplicates (use CRM's built-in deduplication)
- Audit contacts that haven't been touched in 90 days

**Quarterly:**
- Full ICP review — does the database reflect current targeting?
- Purge contacts with zero engagement in 12+ months (or archive)
- Export and cross-check against your enrichment tool for new data

## Output Format
Deliver:
1. CRM Audit Summary (field completion rates, issues flagged)
2. Stale/Invalid Record Cleanup Plan
3. Enrichment Strategy (by tool and priority)
4. Segmentation Framework (for immediate use)
5. Ongoing CRM Hygiene Calendar

## Pro Tips
- A clean CRM is a revenue asset — dirty CRM is a liability that makes every campaign less effective
- Never send outreach from an unenriched list — title mismatches and bad emails kill deliverability permanently
- The 80/20 of CRM enrichment: get email + title right — everything else is secondary
- Use Apollo's "Catch-all" email indicator — these emails may or may not exist, don't include in cold campaigns
- The fastest ROI from CRM cleanup: find contacts in your DB who match your current ICP but were never properly worked — these are your warmest cold leads

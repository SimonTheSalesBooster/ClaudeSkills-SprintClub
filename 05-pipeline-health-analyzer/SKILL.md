# Skill: Pipeline Health Analyzer

## What This Skill Does
Performs a deep diagnostic of a sales pipeline to identify stuck deals, coverage gaps, forecast risk, and velocity issues. Outputs an actionable pipeline review with prioritized deal recommendations, next steps, and a pipeline health score.

## When to Use
- You're doing a weekly or monthly pipeline review
- Your forecast feels unreliable or you're missing your number
- Deals are sitting in stages too long with no movement
- You want to coach your team on which deals to prioritize

## Inputs Required
Before running this skill, ask the user to provide (can be pasted as text or uploaded as CSV/export):
1. **Deal list** — company name, deal value, stage, close date, last activity date, next step
2. **Sales cycle benchmark** — average days per stage (if known)
3. **Monthly/quarterly revenue target**
4. **Current month/quarter close date**
5. **Number of reps (if team pipeline)**

## Step-by-Step Instructions

### Step 1 — Calculate Pipeline Coverage Ratio
```
Pipeline Coverage = Total Pipeline Value ÷ Revenue Target

Healthy coverage ratios:
- 3x = minimum (you need 3x pipeline to hit your number)
- 4–5x = healthy
- 6x+ = risk of sandbagging or poor qualification
- Under 2x = red alert — pipeline emergency
```

Output: Coverage ratio + color-coded status (red/yellow/green)

### Step 2 — Stage Velocity Analysis
For each pipeline stage, calculate:
- **Average days in stage** (from deal data provided)
- **Compare to benchmark** (or industry standard if no benchmark)
- **Flag stalled deals** — any deal sitting 1.5x longer than average in its stage

Standard B2B SaaS benchmarks (adjust based on user's context):
```
Stage                  | Healthy Duration | Stalled Threshold
Discovery/Qualify      | 3–7 days         | >14 days
Demo/Evaluation        | 7–14 days        | >21 days
Proposal/Pricing       | 5–10 days        | >21 days
Negotiation            | 5–14 days        | >30 days
Verbal Commit          | 3–7 days         | >14 days
```

### Step 3 — Deal-Level Risk Scoring
Score each deal from 1–10 on probability of closing this period:

| Risk Factor | Points Deducted |
|-------------|----------------|
| No activity in 14+ days | -2 |
| No defined next step | -2 |
| No economic buyer engaged | -2 |
| Close date is "end of quarter" with no urgency | -1 |
| Deal has been pushed from previous period | -2 |
| No champion confirmed | -1 |
| Missing mutual close plan | -1 |
| Competitor present with no differentiation | -1 |

Score 8–10 = commit | 5–7 = upside | Under 5 = pipeline (not forecast)

### Step 4 — Identify Priority Actions
For each deal, recommend a specific next action based on its risk profile:

**If stalled at Discovery:**
→ "Re-engage with a relevant insight or trigger. Send the 'Have things changed?' message."

**If stalled at Proposal:**
→ "Schedule a proposal review call — proposals don't close themselves. Get the economic buyer on a call."

**If missing next step:**
→ "Reach out today. Use: 'Hey [Name], I want to make sure this stays on track for [date]. Can we confirm [next step]?'"

**If close date keeps slipping:**
→ "Have a direct conversation about what's really in the way. Fake close dates are a forecast killer."

**If no economic buyer:**
→ "Ask your champion: 'When we're ready to move forward, who else would need to weigh in?'"

### Step 5 — Generate Pipeline Health Score & Summary

**Pipeline Health Score (0–100):**
- Coverage ratio: 25 points
- Average deal velocity: 20 points
- % of deals with defined next step: 20 points
- % of deals with economic buyer engaged: 20 points
- Close date distribution (not all stacked at quarter end): 15 points

**Output Summary:**
```
PIPELINE HEALTH REPORT — [Date]

Overall Health Score: [X/100] — [RED / YELLOW / GREEN]

Coverage: [X]x — [Status]
Total Pipeline: $[X]
Target: $[X]
Gap to target: $[X]

CRITICAL DEALS (must close to hit number):
1. [Deal] — $[X] — Action: [...]
2. [Deal] — $[X] — Action: [...]

STALLED DEALS (at risk of slipping):
1. [Deal] — In [Stage] for [X] days — Action: [...]

FORECAST COMMITS:
[List of deals scored 8–10]

THIS WEEK'S FOCUS:
Priority 1: [Specific deal action]
Priority 2: [Specific deal action]
Priority 3: [Specific deal action]
```

## Output Format
Deliver:
1. Pipeline Coverage Ratio with status
2. Stage Velocity Analysis (by stage)
3. Deal Risk Scores (all deals)
4. Priority Action List (top 5 this week)
5. Pipeline Health Score with summary report

## Pro Tips
- Run this review every Monday morning — 30 minutes of pipeline hygiene prevents missed quarters
- Any deal without a next step isn't a deal — it's a wish
- The fastest way to improve forecast accuracy is to ruthlessly remove deals that haven't had activity in 30+ days
- The best indicator of a deal closing is whether the prospect is doing work (sending docs, scheduling calls, looping in stakeholders) — not whether you are
- A pipeline review is a coaching tool, not a status update — always end with "what's the next step and when?"

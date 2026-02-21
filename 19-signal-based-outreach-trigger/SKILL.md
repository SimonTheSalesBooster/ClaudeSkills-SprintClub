# Skill: Signal-Based Outreach Trigger

## What This Skill Does

Scans a list of target accounts or prospects for real-time buying signals — funding rounds, leadership changes, hiring surges, tech stack shifts, and public pain-point signals — then builds a prioritized outreach queue with a personalized first message for each trigger. Turns noise into a reason to call today.

## When to Use

- Your pipeline is cold and you need a reason to reach out that isn't "just checking in"
- You have a list of target accounts but don't know who to contact first
- You want to time outreach to moments of maximum receptivity
- You're running an ABM motion and need to activate accounts at the right moment
- A prospect you've been nurturing just had a material change and it's time to act

## Inputs Required

Before running this skill, ask the user for:

1. **Target account list** — company names, domains, or LinkedIn URLs (10–100 accounts ideal)
2. **Your ICP** — what problem you solve and for whom (title, industry, company size)
3. **Signal sources available** — which of the following the user has access to: LinkedIn (free or Sales Navigator), Crunchbase, G2, Bombora, Apollo, ZoomInfo, or just Google
4. **Time window** — signals from the last 30 days, 60 days, or 90 days?
5. **Outreach channel** — will the triggered message go via email, LinkedIn DM, or phone?

## Step-by-Step Instructions

### Step 1 — Build the Signal Detection Checklist

For each account on the list, check for the following signals in priority order:

**Tier A Signals (Act within 48 hours):**
- New executive hired into a relevant role in the last 90 days (new VP Sales, CRO, CMO, COO, CEO)
- Company announced a funding round in the last 60 days (Series A, B, C, or growth round)
- Company is actively hiring 3+ roles that directly signal the pain you solve
- Merger, acquisition, or spin-off announced

**Tier B Signals (Act within 1 week):**
- Prospect published a LinkedIn post about a challenge you solve
- Company launched a new product or entered a new market
- Company recently rebranded or restructured
- Job posting for a role that would be replaced or augmented by your solution

**Tier C Signals (Add to nurture sequence):**
- Prospect liked or commented on content related to your category
- Company technology stack changed (detected via BuiltWith or Slintel)
- Competitor recently lost the account (if detectable via review sites or network intel)
- Prospect attended a relevant industry conference or webinar

### Step 2 — Score and Prioritize the Queue

Build a Signal Score for each account:

| Signal Type | Points |
|---|---|
| Tier A signal present | 10 pts each |
| Tier B signal present | 5 pts each |
| Tier C signal present | 2 pts each |
| Multiple signals stacked | +3 pts bonus |
| Mutual connection exists | +3 pts |

**Queue tiers:**
- Score 13+ → Contact today
- Score 7–12 → Contact this week
- Score 3–6 → Add to 30-day nurture
- Score 0–2 → Skip for now, revisit next quarter

### Step 3 — Build the Signal Summary Per Account

For each account in the top two tiers, produce a one-paragraph Signal Brief:

- What happened (the signal)
- Why it matters for them (the implication)
- Why it matters for you (the relevance to your solution)
- Who to contact (name, title, LinkedIn URL if available)

### Step 4 — Write the Triggered First Message

For each contact in the top queue, write one personalized opening message using this structure:

**Line 1 — The Signal Hook:** Reference the specific trigger event. One sentence. No fluff.
**Line 2 — The Implication:** Name the challenge or priority this event typically creates. Show you understand their world.
**Line 3 — The Bridge:** One sentence connecting that challenge to what you do — without pitching.
**Line 4 — The Ask:** A low-friction CTA. Not "let's get on a 30-minute call." Ask for a reaction, a yes/no, or a 10-minute conversation.

Keep the total message under 75 words.

### Step 5 — Build the Outreach Calendar

Schedule the triggered outreach:
- Today's queue: accounts scored 13+
- Day 2–3: Follow-up on today's sends with no response + send this week's 7–12 scores
- Day 7: Check for new signals on the full list and refresh the queue
- Day 30: Re-score Tier C accounts for any new signals

## Output Format

Deliver:

1. **Signal Scan Summary** — a table of all accounts with signals found, signal type, and score
2. **Priority Queue** — ranked list with contact name, title, signal, and score
3. **Signal Brief** — one paragraph per top-tier account
4. **Triggered First Messages** — ready-to-send, one per contact, under 75 words
5. **Signal Calendar** — 30-day outreach schedule

## Pro Tips

- New executives are the single highest-converting trigger. A VP who just started a role has a 3–6 month window where they are actively evaluating vendors and making decisions. Hit them in weeks 2–8, not week 1 (too early) or week 16 (too late).
- Stack signals for maximum relevance: a company that raised a Series B AND is hiring a Head of Revenue AND posted about pipeline problems is a 3-signal account — contact them today with all three referenced.
- Don't mention the signal creepily. "I saw you just got hired" lands badly. "Congrats on the new role — I work with a lot of VPs of Sales in your first 90 days" lands well.
- Set a weekly calendar reminder to re-run the signal scan on your full account list. Signals expire. Act within the window or lose the relevance advantage.
- Use LinkedIn job postings as a free intent data source. A company hiring a "Revenue Operations Manager" is telling you they have pipeline problems. A company hiring a "Customer Success Manager" is telling you they have churn risk.

## Example Output Snippet

**Account:** Meridian Software | Signal Score: 18
**Signals:** New CRO hired 6 weeks ago (Tier A, 10 pts) + 4 SDR job postings live (Tier A, 10 pts) + CRO posted about "predictable pipeline" on LinkedIn (Tier B, 5 pts) — stacked bonus applied
**Contact:** James Roark, CRO | linkedin.com/in/jamesroark
**Signal Brief:** Meridian just brought in a new CRO 6 weeks ago and is actively building out their SDR team. This typically signals a mandate to rebuild the outbound motion from scratch — new leader, new budget, new tools decision incoming. Three open SDR reqs confirm they're serious. The window to get in front of James before he's locked into a vendor is now.

**Triggered Message (LinkedIn DM):**
"James — congrats on the CRO role at Meridian. Saw you're scaling the SDR team which usually means the pipeline infrastructure question comes up fast. I work with CROs at similar-stage companies on exactly that. Worth a 10-minute call to see if there's a fit?"

# Skill: Negotiation Conditions Builder

## What This Skill Does
Builds a complete negotiation strategy for any B2B deal — pricing, terms, contract conditions, and concession sequencing. Identifies leverage points, builds walk-away positions, and generates ready-to-use negotiation scripts for every scenario. Helps sellers get better deals without burning relationships.

## When to Use
- A prospect is pushing back on price or terms
- You're about to enter a negotiation and want a plan
- Procurement is involved and asking for concessions
- You want to negotiate better payment terms, contract length, or conditions
- A deal is stalling because of a pricing or scope dispute

## Inputs Required
Before running this skill, ask the user for:
1. **Deal details** — size, scope, what's been proposed
2. **What the prospect is pushing back on** — price, payment terms, contract length, SLAs, other?
3. **Your walk-away point** — the minimum you'd accept (be honest)
4. **What you can flex on** — pricing, payment schedule, start date, add-ons, support level?
5. **Your leverage position** — why do they need you? What's the cost of not buying?
6. **Prospect's deadline or urgency** — do they have a real timeline?

## Step-by-Step Instructions

### Step 1 — Map the Negotiation Landscape
Before negotiating anything, understand the full picture:

**Your Position:**
```
Target outcome (best case):    $[X] | [terms]
Acceptable outcome (likely):   $[X] | [terms]
Walk-away point (minimum):     $[X] | [terms]
```

**Prospect's Position (estimated):**
```
What they asked for:     $[X] or [concession]
What they probably want: $[X] (their real target)
What they can actually afford: $[estimate based on company stage/size]
```

**The Zone of Possible Agreement (ZOPA):**
The range where a deal can happen. If your walk-away is above their maximum, there is no deal — qualify this early.

### Step 2 — Identify Your Leverage Points
Leverage is what gives you power to negotiate without conceding. Build your leverage inventory:

**Strong Leverage (use these):**
- Competitor alternatives aren't as strong (know their weaknesses)
- Prospect has a hard deadline that your solution uniquely solves
- There's a cost/pain to NOT buying (quantify it)
- They've already invested time and resources in your evaluation
- A champion inside has strong advocacy for your solution
- Your implementation timeline is faster than alternatives
- You have reference customers they know and respect

**Weak Signals to Watch For:**
- Deal has been in late stage for 30+ days (leverage erodes with time)
- Multiple competing solutions being evaluated simultaneously
- Budget freeze or reorg — creates urgency to pause, not buy
- Procurement involved with strict cost benchmarks

### Step 3 — Build Your Concession Strategy
Never give concessions for free. Always trade. Build a sequenced plan:

**Concession Sequencing Rules:**
1. Make fewer concessions, not smaller ones — the pattern matters more than the amount
2. Slow down concessions as you go — fast concessions signal you have room
3. Always anchor high — your first number shapes the entire negotiation
4. Get something for every give: "I can do X if you can do Y"

**Concession Hierarchy (give these in order, not all at once):**
```
Tier 1 — Low cost to you, high value to them:
• Extended payment terms (net 60/90 instead of net 30)
• Phased start date (delay implementation, not pricing)
• Add-on feature that costs you nothing to deliver
• Executive sponsor access or dedicated CSM

Tier 2 — Medium cost:
• Additional seats or licenses at no extra charge
• Training or onboarding included at no cost
• Contract term extension at locked pricing

Tier 3 — Last resort:
• Modest price reduction (max 10–15%) with something in return
• A "founding customer" rate IF they agree to a case study, reference, or public logo
• Discount tied to annual prepayment only (protects cash flow)

Never give:
• Discounts without something in return (ever)
• Scope additions without price adjustments
• Extended payment terms AND a discount (one or the other)
```

### Step 4 — Handle the Most Common Negotiation Moves
**"Your price is too high"**
```
Don't: Immediately offer a discount
Do: "Help me understand — too high compared to what? Are you comparing us to a competitor, or is it a budget constraint?"
→ If budget: "What's the number you're working with? Let me see if there's a structure that works."
→ If competitor: "Tell me what they're offering. I want to make sure you're comparing apples to apples."
```

**"Can you do better on price?"**
```
"I'd love to work with you on this. If I can find some flexibility on price, what would you be able to give me in return? For example — could we extend the contract term or move to annual billing?"
```

**"We need net 90 payment terms"**
```
"I can explore that. Net 90 is a meaningful change for us — to make it work, I'd need to adjust the overall investment slightly. Alternatively, if we stay at net 30, I may be able to find more room on price. Which matters more to you?"
```

**"Procurement has a 20% discount policy"**
```
"I understand procurement has benchmarks to hit. Here's the challenge — our pricing already reflects [value/uniqueness]. What I CAN do is restructure the deal so it shows differently on paper. Let's talk about what that might look like."
(Repackage: bundle, phased payment, different line items — same total, different structure)
```

**"We need a pilot before committing"**
```
"I can make a pilot work. To be transparent with you — a free pilot is a significant cost for us. I want to do it in a way that's fair to both sides. If the pilot delivers [agreed-upon success metric], are you ready to sign the full agreement immediately after? Let's put that in writing upfront."
```

**"We're going with someone else unless you match their price"**
```
"I respect that, and I don't want to lose you. Before we talk numbers — help me understand what they're offering. If it's truly apples to apples, I'll be honest with you about what I can and can't do. If it's not, I want to make sure you're making a fair comparison."
```

### Step 5 — Build the Negotiation Script for This Specific Deal
Based on the user's inputs, generate:

**Opening Position Statement:**
```
"[Name], I want to work through this together and find something that works for both of us. Before we get into the details, can I ask — if we can get to the right structure, are you ready to move forward?"
```
→ This anchors commitment before concessions are made.

**Custom Concession Script:**
```
"Here's what I can do: [Tier 1 concession]. That said, I'd need [ask in return] to make that work. Does that help?"
→ If yes: close
→ If not enough: "What would it take to get this done? Help me understand the gap."
```

**Walk-Away Statement:**
```
"[Name], I've done everything I can within what makes sense for us. If [walk-away terms] doesn't work, I respect that — but I'm not in a position to go further. I'd rather be transparent with you now than start a relationship on terms that don't work for either of us."
```

### Step 6 — Output the Negotiation Brief
```
NEGOTIATION BRIEF — [Deal Name]

Your anchor: $[X] at [terms]
Walk-away: $[X] at [terms]
ZOPA estimate: $[range]

THEIR MAIN ASK: [what they want]
ROOT CONCERN: [budget / timeline / risk / authority]

YOUR LEVERAGE:
1. [Leverage point 1]
2. [Leverage point 2]

CONCESSION SEQUENCE:
Move 1: [Low-cost concession + what you ask for in return]
Move 2: [Medium-cost concession + what you ask for in return]
Last resort: [Price adjustment + condition]

OPENING LINE: [Ready to use]
FIRST CONCESSION SCRIPT: [Ready to use]
WALK-AWAY LINE: [Ready to use]
```

## Output Format
Deliver:
1. Negotiation Landscape Map (your position, their position, ZOPA)
2. Leverage Inventory
3. Concession Sequence (tiered, with trades)
4. Scripts for the 3 most likely objections they'll raise
5. Full Negotiation Brief (print/meeting-ready)

## Pro Tips
- The party with the most options wins. Always be building pipeline in parallel — it protects your walk-away position.
- Whoever names a number first in a negotiation anchors it. If they go first, they own the anchor. If you go first, make it aggressive.
- Silence after an ask is your most powerful tool — most reps fill it with concessions they didn't need to make
- Never negotiate against yourself ("How about I throw in X and Y and Z...") — wait for their counter
- The best deals feel like both parties got something. Help the prospect feel like they won — give them a visible win that costs you very little.
- If procurement is involved and unnamed — get them in the room. Invisible stakeholders kill more deals than bad pricing.

---
title: "The Shower That Ate Your Engineering Budget"
date: 2025-11-30
author: Dan Zrobok
header:
  teaser: /assets/images/metronome.png
tags: [boringops, cloud, cost, complexity, vendors]
excerpt: "You threw out a $500 bathtub and ended up in a communal shower where the faucet, soap, water, and air are all billable events."
layout: single
---
Most places toss the baby out with the bathwater, only to realize the water’s gone, the baby’s grown up, and a vendor stole the bathtub.

Then leadership announces the **upgrade**: showers for everyone.

**Clap, please.**

After months of expensive process remodeling, you end up in a cold communal shower where every scrub costs more.

## The Bathtub: Stable, Cheap, and Apparently Unacceptable

**2005: You Own a Bathtub**

Cost you $500. That's it. You clean it when it needs cleaning. Take as many baths as you want. Nobody's watching. It just... works. Same way it did yesterday, same way it'll work tomorrow. Dead simple.

**2010: "Bathtubs Don't Scale"**

The vendor arrives with a pitch deck.

> “What if you need to bathe 1000 people? Or there’s a sudden bathing surge event? Hmm... just one bathtub? Sounds like a single point of failure... risky in today's customer expectation economy..."

The seed of doubt is planted. 

Your bathtub, which has worked perfectly for years, suddenly feels inadequate.

**2015: The Migration**

- Flag the bathtub as “legacy”
- Force everyone to shower at the Communal Facility™: us-east-shower-2
- Celebrate the "shower-native" architecture
- Write a blog post about your "transformation journey"
- Add new teams to manage the “modern hygiene platform”
- "Pay only for what you use!" they promise
- "It's more flexible!" they assure
- Tear out the bathtub “to reclaim savings”
- Convert the old bathroom into a meeting room with bad lighting

**2020: The Bill Arrives**
```
Monthly Shower Statement:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Base access fee:               $5/month
Per-shower charge:             $0.05/shower × 30 showers
Hot water premium:             $0.25/shower × 30 showers
S3oap dispenser fee:           $0.10/pump × 120 pumps
Towel rental:                  $0.50/use × 30 uses
Peak-time surcharge:           $1/shower × 12 showers
Warm Shower Reservation Fee:   $5/month
Water egress fee:              $0.09/L x 200 litres (drainage)
Humidity Monitoring:           $0.25/GB x 12GB (1 minute intervals)
DropletWatch Logging:          $0.002/event × 1,240 events
Other Fixture Utilization:     $2/month (sinks, toilets, mirrors)
Support tier fee:              $5 (access to shower attendants and maintenance)

Total this month:              $88.48
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

Someone does the math.

You're spending $1,062 a year on communal showers.
The old bathtub cost $500. Once.

You could have bought two new deep soaking bathtubs for what you’re paying annually. And the worst part?

The vendor didn’t upsell you. You upsold yourself. Every add-on looked like “best practice,” so you clicked them all.

Now you’re paying nearly a hundred bucks a month for something that used to be free *and* calling it progress.

**2025: The New Normal**

Showers cost over a thousand bucks a year and nobody blinks. New hires think this is just how the world works. You show up to the facility and there's a lenghty waitlist. The vendor? They just raised prices 12% to fund a state-of-the-art shower facility in Prague you'll never use.

## The Soap-Per-Scrub Model

The real genius isn't just that showers are expensive. It's that the cost is **designed to be incomprehensible**.

### What They Promised

> "Pay only for what you use! So efficient! No waste!"

### What It Actually Means

You cannot predict your monthly bill. Every action triggers multiple micro-charges that seem insignificant individually but compound into shocking totals.

## The Two Models Compared

### The Bathtub (On-Premises)

**Upfront cost:** $500  
**Monthly cost:** $0  
**10-year total:** $500  

**Characteristics:**

The cost is clear and never changes. You can use it as much as you need. Total control over everything. Your privacy is yours. No vendor owns you. And it keeps working even when the internet dies.

### The Communal Shower (Cloud)

**Upfront cost:** $0  
**Monthly cost:** $88.48  
**10-year total:** $10,617.60  

**Characteristics:**

Costs fluctuate wildly. Capacity is unlimited in theory but priced to hurt. The vendor controls what features exist. Your privacy is whatever their policy says it is this quarter. You're completely locked in. And when their service goes down, so do you.

**The difference: $10,117.60**

That's not rounding error. That's **2,023.52% more expensive** for the "flexible" solution.

## Why You Can't Just Go Back

> "Okay, so we made a mistake. Let's just reinstall the bathtub."

If only it were that simple.

### The Technical Barriers

1. **The water pipes were removed** - Classified as “idle resources” and decommissioned
2. **The team lost bathing knowledge** - Everyone only knows showers
3. **The data is in their format** - Everything is stored in proprietary shower-log format
4. **Dependencies everywhere** - 47 systems assume shower availability APIs

### The Political Barriers

1. **Someone's promotion depended on the migration** - Admitting failure is career suicide
2. **The board was told this was "modernization"** - Reversing looks like incompetence
3. **The industry validates the choice** - Every conference says communal showers are "best practice"
4. **Sunk cost fallacy** - "We've already invested so much in the migration"

### The Organizational Barriers

1. **No budget for "moving backward"** - Innovation budget only flows one direction
2. **The old bathtub expertise is gone** - The plumber was managed out years ago
3. **New hires expect showers** - "You use a bathtub? How quaint"
4. **Vendor has leverage** - "Migration off our Communal Facility™? Good luck"
5. **The bathroom is gone** - It’s now a meeting room booked solid for the next decade

You're stuck taking expensive showers.

## The Vendor's Dream

The communal shower is perfect for vendors because it fixes their biggest problem: **customers who stop paying**.

In the bathtub world, you pay $500 once, and you’re done. In the shower world, you pay every month, forever, and you can’t leave.

The old model gives vendors a one-time $500 sale. The new model turns hygiene into a **perpetual revenue stream** measured in annual recurrences, expansions, surcharges, and “operational cost adjustments.”

You didn’t buy a shower. You bought a subscription the vendor can change whenever they feel like it.

### The Vendor Playbook

**Step 1: Create Doubt**

First they make you question what you have. "Bathtubs don't scale." "What about flexibility?" "Everyone else is using showers." "Don't get left behind." Your bathtub worked fine yesterday, but now it feels like a liability.

**Step 2: Hide True Costs**

They offer free migration. Show you entry pricing that looks reasonable. The actual cost structure is designed to be incomprehensible. They keep saying "pay only for what you use" like it's a feature instead of a warning.

**Step 3: Create Lock-In**

Everything gets stored in their proprietary format. Your other systems start depending on their APIs. The sunk cost piles up. By the time you realize you want out, the exit costs are astronomical.

**Step 4: Let You Increase Your Own Prices**

They hook you with low entry pricing. Then they sit back and watch. You enable logging because it seems smart. Add monitoring because what if something breaks. Upgrade support because downtime is scary. Every feature looks like best practice. A year later you're paying triple and the vendor didn't have to sell you anything. You sold yourself.

**Step 5: Repeat**

A year later they announce "Shower 2.0 Managed Service with Integrated, AI-Powered, Hyper-Personalized Hygiene Mesh and Built-in FinOps Compliance." Your current shower still works fine, but the new version promises to fix all those annoying issues. Y'know, the ones that only exist because you're using their shower in the first place. 

The waitlists disappear (for now). The billing becomes a little clearer (but somehow, more line items?). You migrate because the pain is real, and the solution is right there, sparkling. They charge you for the upgrade. Eighteen months later, Shower 3.0 gets announced. The cycle never ends.

Has your business moved forward or has the vendors balance sheet flourished instead? 

## The Optimization Theatre

Eventually someone notices the shower bill is out of control.

Leadership hires a **“Shower Cost Optimization Consultant”** for a $50,000 engagement to reduce the $10,617.60/year shower bill.

You are now spending **$60,000** on showers.

The consultant's recommendations:

1. **“Right-size your showers”** — take shorter showers. It’s 15% cheaper to machine-gun the water on and off than let it run.  
2. **“Use reserved shower capacity”** — commit to 100 showers/month for a 12.7% discount you’ll never fully use  
3. **“Leverage spot shower pricing”** — shower at 3 AM and pray the rate doesn’t spike when the clubs let out  
4. **“Implement shower governance”** — require VP approval every time you want hot water  
5. **“Adopt a FinOps culture”** — install a frowny wall timer that flashes red and sighs loudly when you exceed your 75.3s shower budget

Notice what’s NOT recommended: **get a bathtub.**

The consultant is paid to optimize the shower, not question why you’re showering at all.

After six months, you’ve reduced the annual shower bill from $1,062 to $955.80. The water is mostly cold now, but people only complain in whispers because the shower debate exhausted social capacity.

**Savings: $106.20/year**  
**Consultant cost: $50,000**  
**Net result: you’re still spending way more than before**

But... Now you have beautifully color-coded shower dashboards and a CTO-grade red button that can terminate a shower on demand, so that’s something.

## The Conference Circuit

**Conference Talk Title:**  
"From Bathtub Monolith to Communal Shower Mesh: A Transformation Success Story"

**Abstract:**  
> Join us as we share our journey from legacy bathtub architecture to a modern, shower-native communal platform. We’ll cover cost optimization, shower observability, and our migration to a fully managed Shower Mesh. Learn how we achieved 99.9% SA (shower availability) while reducing TTC (time-to-clean) by 40%.

**What the talk includes:**
- Impressive architecture diagrams  
- Metrics showing “improvement” (showers: 4 min → 2.41 min)  
- Stories of conquering “technical debt” (the bathtub)  
- Team photos of the “transformation squad” (no one is smiling)  
- A vendor logo on every slide  

**What the talk doesn’t mention:**
- Showers used to cost $0, now cost $73.80/month (post-expensive consulting)  
- The old bathtub worked perfectly  
- Three engineers quit during the migration  
- Time-to-clean improvement is meaningless (you were already clean)  
- The real “technical debt” was replacing something that worked  

**Audience reaction:**  
> “Wow, we’re so behind. We need communal showers too. Our bathtub is clearly holding us back.”

And the cycle continues.

## The Boring Alternative

The other company kept the bathtub from 2005. It works the same as it always did. Zero monthly cost. Nobody wastes time thinking about it. The entire team focuses on building product instead of managing hygiene infrastructure.

**After 10 years:**

**Bathtub company total cost: $500**  
**Shower company total cost: $10,617.60**

The shower company? They've got the impressive architecture diagrams, the conference talks, the vendor partnerships, the engineers padding their resumes with "shower-native" experience. Looks great in a deck.

The bathtub company? More cash, more capacity, simpler ops, people who sleep through the night, and an actual competitive edge.

One of these companies builds product. The other builds shower dashboards. Guess who wins.

## The Sales Pitch, Decoded

When a vendor sells you on migrating from bathtubs to showers, here's the actual translation:

| What They Say                 | What They Mean                           |
|------------------------------|-------------------------------------------|
| "Eliminate operational burden"| "Shift your burden to us and pay for it" |
| "Pay only for what you use"   | "Pay for everything you didn't notice"    |
| "Infinite scalability"        | "Infinite billing at scale"               |
| "Industry best practice"      | "The thing that makes us the most money"  |
| "Cloud-native architecture"   | "You belong to us now"                    |
| "Modern infrastructure"       | "More expensive infrastructure"           |
| "Digital transformation"      | "Our margins go up, yours go down"        |
| "Future-proof your business"  | "Future-lock your spending"               |


The entire pitch is designed to make you feel **inadequate** about what you have and **optimistic** about what they're selling.

## The Real Questions

Before you rip out your bathtub, ask:

### Business Questions

1. **What problem are we solving?** (Be specific, not theoretical)
2. **What's the total cost over 10 years?** (Not just migration cost)
3. **Can we go back if this fails?** (Probably not)
4. **What's the opportunity cost?** (What else could we build with this time and money?)

### Technical Questions

1. **Is our current system actually failing?** (Or just unfashionable?)
2. **What's the carrying cost of complexity?** (How much permanent overhead are we adding?)
3. **Do we have expertise for the new thing?** (Or are we learning on production?)
4. **What's the blast radius if this breaks?** (Can we contain failure?)

### Cultural Questions

1. **Why do we want to do this?** (Honest answer: resume building? peer pressure? actual need?)
2. **Who benefits from this change?** (The team? The business? The vendor? Individual careers?)
3. **What are we sacrificing?** (Simplicity? Predictability? Budget?)
4. **Can we articulate success criteria?** (How will we know if this was worth it?)

If you can't answer these clearly, you're not ready to throw out the bathtub.

## The BoringOps Position

BoringOps isn't against change. It's against **wasteful change**.

If your bathtub is broken, fix it or replace it. If it works, **leave it alone** and spend your energy on something that matters.

The most valuable engineering work is often the work you **don't do**.

Don't migrate because everyone else is migrating. Don't chase architectural fashion. Don't let vendors manufacture urgency. And don't ever confuse movement with progress.

**Keep the bathtub, the baby and the bathwater.**

And if a vendor tries to sell you a communal shower, simply state:

> 'We prioritize simplicity in architecture, and our bathtub is stable, fully documented, and it was paid off twenty years ago'.

## Epilogue: The Subscription Economy

The communal shower is just one example of a broader pattern: **converting ownership into subscription**.

- Software: Buy once → SaaS forever
- Infrastructure: Own servers → Rent compute
- Tools: Install locally → Cloud-based subscription
- Music: Buy albums → Streaming fee
- Transportation: Own car → Ride share
- Housing: Own home → Rent apartment

The pitches are all the same, but so is the reality:

- **You pay forever**
- **You own nothing**
- **Vendor controls features**
- **Price increases are inevitable**
- **You can't leave**

The bathtub is not just a metaphor for infrastructure.

It's a metaphor for every choice between ownership and subscription, between control and convenience, between upfront investment and eternal payment.

**Choose carefully**.

The monthly bill always seems reasonable until you're taking an ice-cold 3 AM shower in Ohio to stay under the **new CTO**'s budget. 

---

**boring (adj.)**: Having a bathtub that works, costs nothing monthly, and lets you focus on actual problems instead of shower optimization strategies.
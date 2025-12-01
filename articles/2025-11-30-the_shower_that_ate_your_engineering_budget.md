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

Then leadership announces the “upgrade”: showers for everyone. **Clap, please**.

And after months of expensive process remodeling, you end up in a cold communal shower where every scrub costs more.

## The Bathtub: Stable, Cheap, and Apparently Unacceptable

**2005: You Own a Bathtub**

- Upfront cost: $500
- Maintenance: clean it yourself
- Capacity: unlimited baths
- Privacy: it's in your house
- Predictable: works the same every day

**2010: "Bathtubs Don't Scale"**

The vendor arrives with a pitch deck.

- “What if... you need to bathe 1000 people?”
- “What if... there’s a sudden bathing surge event?”
- “What if... your single point of failure bathtub... fails?”

The seed of doubt is planted. 

Your bathtub, which has worked perfectly for years, suddenly feels inadequate.

**2015: The Migration**

- Flag the bathtub as “legacy”
- Force everyone to shower at the Communal Facility™
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
Soap dispenser fee:            $0.10/pump × 120 pumps
Towel rental:                  $0.50/use × 30 uses
Peak-time surcharge:           $1/shower × 12 showers
Warm Shower Reservation Fee:   $5/month
Water egress fee:              $0.09/L x 200 litres (drainage)
Humidity Monitoring:           $0.25/GB x 12GB (1 minute intervals)
Hygiene Event Logging:         $0.002/event × 1,240 events
Other Fixture Utilization:     $2/month (sinks, toilets, mirrors)
Support tier fee:              $5 (access to shower attendants and maintenance)

Total this month:              $88.48
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

Someone does the math.

You're spending $1,062 a year on communal showers.
The old bathtub cost $500. Once.

You could have bought two new deep soaking bathtubs for what you’re paying annually. 

And the worst part?

The vendor didn’t upsell you: you upsold yourself.

Every add-on looked like “best practice,” so you clicked them all.

Now you’re paying nearly a hundred bucks a month for something that used to be free *and* calling it progress.

**2025: The New Normal**

- Everyone accepts that showers cost over a grand a year  
- New hires assume communal showering is normal  
- You show up to shower and discover there’s a waitlist  
- The vendor bumps prices 12%, “due to increased operational costs” (they’re building a shower facility in Prague you’ll never use)

## The Soap-Per-Scrub Model

The real genius isn't just that showers are expensive. It's that the cost is **designed to be incomprehensible**.

### What They Promised

> "Pay only for what you use! So efficient! No waste!"

### What It Actually Means

You cannot predict your monthly bill. Every action triggers multiple micro-charges that seem insignificant individually but compound into shocking totals.

The charges are small enough to ignore in the moment but large enough to devastate your budget by month's end.

## The Two Models Compared

### The Bathtub (On-Premises)

**Upfront cost:** $500  
**Monthly cost:** $0  
**10-year total:** $500  

**Characteristics:**
- Cost visible and predictable
- Capacity unlimited within reason
- Complete control
- Privacy guaranteed
- No vendor lock-in
- Works during internet outages

### The Communal Shower (Cloud)

**Upfront cost:** $0  
**Monthly cost:** $88.48  
**10-year total:** $10,617.60  

**Characteristics:**
- Cost unpredictable and variable
- Capacity theoretically unlimited (but expensive)
- Limited control (vendor decides features)
- Privacy dependent on vendor policies
- Complete vendor lock-in
- Stops working if vendor has outage

**The difference: $10,117.60**

That's not rounding error. That's **2,023.52% more expensive** for the "flexible" solution.

## Why You Can't Just Go Back

"Okay, so we made a mistake. Let's just reinstall the bathtub."

If only it were that simple.

### The Technical Barriers

1. **The water pipes were removed** - Classified as “idle resources” and decommissioned
2. **The team lost bathing knowledge** - Everyone only knows showers
3. **The data is in their format** - Everything is stored in proprietary shower-log format
4. **Dependencies everywhere** - 47 systems assume shower availability

### The Political Barriers

1. **Someone's promotion depended on the migration** - Admitting failure is career suicide
2. **The board was told this was "modernization"** - Reversing looks like incompetence
3. **The industry validates the choice** - Every conference says communal showers are "best practice"
4. **Sunk cost fallacy** - "We've already invested so much in the migration"

### The Organizational Barriers

1. **No budget for "moving backward"** - Innovation budget only flows one direction
2. **The old bathtub expertise is gone** - The plumber was managed out years ago
3. **New hires expect showers** - "You use a bathtub? How quaint"
4. **Vendor has leverage** - "Migration off our Communal Facility? Good luck"
5. **The bathroom is gone** - It’s now a meeting room booked solid for the next decade

You're stuck taking expensive showers.

## The Vendor's Dream

The communal shower is perfect for vendors because it fixes their biggest problem: **customers who stop paying**.

In the bathtub world, you pay $500 once, and you’re done.  
In the shower world, you pay every month, forever, and you can’t leave.

The old model gives vendors a one-time $500 sale.  
The new model turns hygiene into a **perpetual revenue stream** measured in annual recurrences, expansions, surcharges, and “operational cost adjustments.”

You didn’t buy a shower.  
You bought a subscription the vendor can raise whenever they feel like it.

### The Vendor Playbook

**Step 1: Create Doubt**
- "Bathtubs don't scale"
- "What about flexibility?"
- "Everyone else is using showers"
- "Don't get left behind"

**Step 2: Hide True Costs**
- Offer free migration
- Show low entry pricing
- Make cost structure incomprehensible
- Emphasize "pay only for what you use"

**Step 3: Create Lock-In**
- Proprietary formats
- Ecosystem dependencies
- Sunk cost psychology
- High exit costs

**Step 4: Increase Prices**
- Start low to win business
- Raise prices after migration
- Customer can't leave
- Profit

**Step 5: Repeat**
- Announce "Shower 2.0"
- Deprecate old shower
- Force another migration
- Charge for the upgrade

## The Optimization Theatre

Eventually someone notices the shower bill is out of control.

Leadership hires a **“Shower Cost Optimization Consultant”** for $50,000 to reduce the $10,617.60/year shower bill.

You are now spending **$60,000** on showers.

The consultant's recommendations:

1. **“Right-size your showers”** — take shorter showers. It’s 15% cheaper to machine-gun the water on and off than let it run.  
2. **“Use reserved shower capacity”** — commit to 100 showers/month for a 12.7% discount you’ll never fully use  
3. **“Leverage spot shower pricing”** — shower at 3 AM and pray the rate doesn’t spike when the clubs let out  
4. **“Implement shower governance”** — require VP approval every time you want hot water  
5. **“Adopt a FinOps culture”** — install a frowny wall timer that flashes red and sighs loudly when you exceed your 75.3s shower budget

Notice what’s NOT recommended: **get a bathtub.**

The consultant is paid to optimize the shower, not question why you’re showering at all.

After six months, you’ve reduced the annual shower bill from $1,062 to $955.80. The water is mostly cold now, but people only complain in whispers because no one wants to reopen the shower debate.

**Savings: $106.20/year**  
**Consultant cost: $50,000**  
**Net result: you’re spending more than before**

But now you have beautifully color-coded shower dashboards and a CTO-grade red button that can end a shower on demand, so that’s something.

## The Conference Circuit

**Conference Talk Title:**  
"From Bathtub Monolith to Communal Shower Mesh: A Transformation Story"

**Abstract:**  
> Join us as we share our journey from legacy bathtub architecture to a modern, shower-native communal platform. We’ll cover cost optimization, shower observability, and our migration to a fully managed Shower Mesh. Learn how we achieved 99.9% shower availability while reducing time-to-clean by 40%.

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

Meanwhile, a small company kept their bathtub.

**Their infrastructure:**
- Same bathtub installed in 2005
- Works exactly the same
- Costs $0/month
- Nobody thinks about it
- Team focuses on building product

**After 10 years:**

**Bathtub company total cost: $500**  
**Shower company total cost: $10,617.60**

The shower company has:
- More impressive architecture diagrams
- Better conference presentations  
- Modern vendor relationships
- A shower-native resume builder for engineers

The bathtub company has:
- More money
- More engineering capacity
- Less operational complexity
- Better sleep
- Actual competitive advantage

**Question:** Which company can invest more in their actual product?

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

- Don't migrate because everyone else is
- Don't chase architectural fashion
- Don't let vendors create urgency
- Don't confuse movement with progress

**Keep the bathtub. Keep the baby. Keep the bathwater.**

And if a vendor tries to sell you a communal shower, ask them why they're so interested in turning your $500 bathtub into their $10,000 revenue stream.



## Epilogue: The Subscription Economy

The communal shower is just one example of a broader pattern: **converting ownership into subscription**.

- Software: Buy once → SaaS forever
- Infrastructure: Own servers → Rent compute
- Tools: Install locally → Cloud-based subscription
- Music: Buy albums → Streaming fee
- Transportation: Own car → Ride share
- Housing: Own home → Rent apartment

In every case, the pitch is the same:
- "More flexible!"
- "Lower upfront cost!"
- "Always up to date!"
- "No maintenance burden!"

And in every case, the reality is the same:
- **You pay forever**
- **You own nothing**
- **Vendor controls features**
- **Price increases are inevitable**
- **You can't leave**

The bathtub is not just a metaphor for infrastructure.

It's a metaphor for every choice between ownership and subscription, between control and convenience, between upfront investment and eternal payment.

Choose carefully.

The monthly bill always seems reasonable until you're taking an ice-cold 3 AM shower to stay under budget. But it’s the 10-year cost and lost efficiency that should make you shiver.

---

**boring (adj.)**: Having a bathtub that works, costs nothing monthly, and lets you focus on actual problems instead of shower optimization strategies.
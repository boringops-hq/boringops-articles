---
title: "BoringOps: The Uncomfortable Truths Nobody Wants to Hear"
#excerpt: "The hardest part of doing boring work is explaining why you didn't do exciting work."
header:
  teaser: /assets/images/metronome.png
tags: [consistency, infrastructure]
layout: single
classes: wide
---

> The hardest part of doing boring work is explaining why you didn't do exciting work.

Let's stop pretending BoringOps is just a philosophy problem. It's an economic problem, a political problem, and a career problem. You can believe in stability all you want—the system you work in is designed to punish you for it.

Here's what actually happens when you try to practice BoringOps in the real world.

## Truth #1: Your Career Depends on Visible Change

You know what gets you promoted? Launching things. Migrating things. "Leading the initiative to modernize our deployment pipeline." You know what doesn't? "Kept the Jenkins instance running for another year because it works fine."

The performance review has no checkbox for "prevented unnecessary work." Your manager needs to write a narrative about your impact. "Sarah maintained stability" is not a narrative. "Sarah led our migration to Kubernetes, reducing deployment time by 40%" is a narrative. Never mind that the old system deployed in 4 minutes and the new one deploys in 2.4 minutes and took six months to build.

BoringOps asks you to optimize for the business. Your career optimization function is different. Until companies learn to reward stability as much as they reward transformation, this tension won't resolve.

**What this means**: If you choose boring, choose it with eyes open. You might do the right thing for the company and the wrong thing for your next job title. That's not noble. It's just math.

## Truth #2: "Nobody Got Fired for Buying IBM" Is Still True

The safest career move is doing what everyone else is doing. If your infrastructure falls over because you're running a bespoke stack that seemed sensible, you're an idiot. If it falls over because you're running the same thing as everyone else, well, AWS had an outage. What could you do?

BoringOps often means choosing the boring-but-proven over the exciting-but-standard. That's career risk. When you defend your decision to stick with Postgres instead of adopting the latest distributed database that your competitors use, you better be right. If you're wrong, you're the person who was "too conservative" and "resistant to innovation."

The herd provides cover. Boring provides exposure.

**What this means**: Being boring requires more confidence than being trendy. You need to be right more often because you have fewer excuses when you're wrong.

## Truth #3: Vendors Will Eat You Alive

Every SaaS company, every consultant, every conference talk is selling the same story: your current approach is insufficient. Here's the gap you didn't know you had. Here's the tool that fills it.

They're not wrong to sell. They're wrong about how often you need to buy.

But here's the trap: if you're a decision-maker and you *don't* adopt the new thing, and then something goes wrong, people will ask why you didn't have "industry standard" tooling. The vendor ecosystem creates a constant tax on doing nothing. Standing still feels like falling behind because everyone's shouting about how far ahead they're getting.

BoringOps means ignoring most of what you hear at conferences. It means watching your peers adopt tools you don't need. It means being comfortable with FOMO as a permanent condition.

**What this means**: You have to develop an immune system against solutions looking for problems. Most teams don't have this. It's easier to buy the thing than to justify not buying the thing.

## Truth #4: Hiring Is a Nightmare

Post a job that says: "We use Postgres, Rails, and deploy with Capistrano. Our infrastructure hasn't changed in three years. You will mostly fix small bugs and respond to occasional issues."

Now post one that says: "We're building a modern microservices platform on Kubernetes with React and GraphQL. Greenfield opportunity to shape our technical future."

Which one gets more applicants?

Boring companies struggle to hire because engineers optimize for resume lines, not for sustainable work. The candidate who wants to learn Kubernetes won't join your boring shop. The candidate who just wants stability is... well, they're probably already employed and not looking.

You end up with two choices: hire people who want excitement and watch them get bored and leave, or hire people who value stability and accept a smaller talent pool.

**What this means**: BoringOps has a talent ceiling. You can't just decide to be boring—you have to build a team that can tolerate it. That's harder than it sounds.

## Truth #5: Startups Can't Afford Boring

If you're pre-product-market-fit, boring is death. You need to move fast, try things, pivot. Your infrastructure should be held together with duct tape because you might throw the whole thing away next month.

BoringOps is a luxury of success. It only works when you've found something worth stabilizing. Before that, premature boring is just premature optimization with a different name.

The hard part? Knowing when to switch. Most teams stay in chaos mode too long. Some teams prematurely optimize. There's no clear signal for when boring becomes the right move.

**What this means**: BoringOps is not universal advice. If you're still figuring out what you're building, you should probably keep things exciting. The trick is recognizing the transition.

## Truth #6: Leadership Wants a Story

Your CTO needs to go to the board and talk about technical progress. "We did nothing this quarter because everything already works" is not a winning message. Leadership needs wins. Stability is invisible until it breaks.

This creates a perverse incentive: executives want evidence of technical investment. The quieter your ops become, the harder it is to justify your headcount. Teams that constantly ship visible improvements look productive. Teams that maintain invisible stability look... expendable?

So you end up doing projects you don't need, not because they're necessary, but because you need to prove you're doing something.

**What this means**: BoringOps requires executive buy-in that most companies don't have. Without it, you'll get pressured to create motion even when stillness is the right answer.

## Truth #7: The Industry Has Amnesia

Every few years, the industry forgets the lessons it learned and has to relearn them expensively.

Microservices? We learned this in the SOA era. Serverless? We learned this with CGI scripts. Kubernetes? We learned this with Mesos and YARN and the datacenter automation before that.

The pattern repeats: new technology promises to solve old problems, creates new problems, eventually settles into boring stability, and then gets replaced by the next thing that promises to solve the old problems.

BoringOps means opting out of this cycle. It means using last decade's boring solution instead of this decade's exciting one. But the industry doesn't reward institutional memory. It rewards being early to the next thing.

**What this means**: You'll constantly feel outdated even when you're making the right call. The only way to deal with this is to stop caring about feeling current.

## Truth #8: Boring Requires Saying No, Constantly

The hardest part of BoringOps isn't technical. It's social.

It's saying no when a senior engineer wants to rewrite the deployment system. It's saying no when everyone's excited about the new observability platform. It's saying no when a competitor announces they're using some exciting new stack.

Every no feels like you're being the person who "doesn't get it." Every no requires justification. Every no is an argument you have to win.

Exciting only requires one yes. Boring requires infinite nos.

**What this means**: BoringOps is exhausting in a different way than exciting ops. You're not tired from doing too much. You're tired from defending doing enough.

## So What Do You Actually Do?

If you still want to practice BoringOps after reading all this, here's what it actually looks like:

**Accept the career trade-off**: You might advance slower. You might have fewer impressive bullets on your resume. If you're okay with that, continue. If you're not, don't pretend. Chase the exciting work and own it.

**Build a moat of documentation**: When you don't do something, document why. "We evaluated X and chose not to adopt it because Y" is evidence. It's cover for later. It's proof you were thoughtful, not lazy.

**Quantify the invisible**: Track what didn't happen. Uptime. Time saved not maintaining systems. Hours not spent in incidents. Make boring measurable so it becomes visible.

**Find allies in leadership**: You need at least one executive who understands that stability is valuable. Without that, you're fighting culture alone.

**Be ready to be wrong**: Sometimes the exciting new thing really is better. Sometimes boring is just stubbornness. Stay curious enough to know the difference.

**Choose your battles**: You can't be boring about everything. Pick what matters most and let other things be exciting. Maybe your deployment pipeline is boring but your product features are experimental. Balance the portfolio.

**Hire for values, not skills**: You need people who value sustainable work over resume-building. That's a cultural fit question, not a technical one.

## The Real Revolution

BoringOps isn't quiet because it's calm. It's quiet because it's hard to explain, hard to sell, and hard to sustain in a system built to resist it.

The real revolution isn't choosing boring technology. It's building a company culture that rewards preventing problems as much as solving them. It's convincing leadership that operational silence is success. It's creating career paths that don't require constant visible motion.

That's not a philosophy shift. That's a power shift. And power doesn't shift because someone wrote a manifesto.

It shifts when enough people get tired of the chaos and demand something different. When enough CTOs realize their best engineers are burning out from excitement. When enough companies discover that their most valuable infrastructure is the stuff nobody thinks about anymore.

Until then, BoringOps remains what it is: the right answer that most people can't afford to choose.

---

**boring (adj.)**: the thing you choose when you're willing to sacrifice your career momentum for the company's stability. See also: principle, cost.
---
title: "Pillar 2: Simplicity"
excerpt: "Simplicity removes everything that makes a system harder to understand, repair, and trust. If you cannot sketch it on a napkin, it is too complex."
header:
  teaser: /assets/images/metronome.png
tags: [pillars, complexity, architecture]
layout: single
classes: wide
author: Dan Zrobok
date: 2025-08-02
---

> "Complexity is not clever. It is how outages introduce themselves."

Simplicity is the second pillar of BoringOps because it decides whether a system survives contact with reality. 

While consistency gives predictability, simplicity determines whether the system can be understood and repaired when predictability collapses.

Simplicity is not aesthetics. It is the refusal to add anything that makes a system harder to understand, fix or trust. A system can be powerful and still be simple. The parts that make it complex are usually the parts nobody needed.

Simplicity is the discipline that prevents systems from punishing the people who must keep them alive.

## The Real Source of Complexity

Complexity does not come from product requirements. It comes from incentives.

Engineers optimize for elegance over operability. Leaders chase modernity. Vendors sell futures that depend on adopting their model. These pushes accumulate into architectures that look impressive and behave unpredictably.

Complexity feels responsible at the time. It feels like diligence. In reality it produces systems that function only while their assumptions hold. Once those assumptions shift, complexity becomes a liability.

## When Simplicity Breaks

Complexity creates patterns that drain capacity and hide risk.

### The Abstraction Nobody Uses

A layer added for a future that never arrived. No one uses it, but it remains in the critical path adding latency and confusion, serving no one.

### The Config Explosion

Thirty flags to control behavior that should have been one decision. Every flag is a branch no one tests. The system becomes impossible to reason about because nobody knows which combination is running.

### The Invisible Dependency

A service nobody remembers until it fails. Added quietly, documented nowhere, and understood only by the person who left. It surfaces at 2 AM when the cascade begins.

> never forget the ['left-pad'](https://en.wikipedia.org/wiki/Npm_left-pad_incident) debacle

All three share one cause. Complexity was allowed to accumulate without earning its place.

## Complexity Is Debt That Matures at Night

Complexity starts charging interest the moment it enters a system. You build it. You operate it. Then someone new has to understand it. That moment reveals how fragile it always was.

Complexity ages quickly. It becomes a pile of half-remembered decisions that nobody wants to disturb. Deployments feel risky. Incidents become archaeology. People stop touching the system because touching it feels unsafe.

This is not normal work. It is accumulated cognitive debt.

## BoringOps Rejects Clever Architecture

Clever architectures fail where simple architectures survive. Clever solutions work under controlled conditions. They rot because their assumptions drift quietly over time. When they fail, they require heroics to recover.

Simplicity is not primitive. Advanced systems can be simple when every component earns its keep and no piece exists for show. 

Power does not require confusion.

## The Napkin Test

If you cannot sketch the core of your system on a napkin and walk a new engineer through it in five minutes, it is too complex.

If only one person can draw a version that matches reality, you do not have a system. You have a human dependency. That is not resilience. It is fragility.

## Complexity Hiding in Plain Sight

> In one incident, a client's ESB looked flawless. Logs clean. Yet consumers received corrupted responses. Hours later someone remembered a forgotten vendor response cache outside the network. It truncated payloads. It existed only in production.

This is complexity. It hides until the worst possible moment.

## The Organizational Cost of Complexity

Complexity does not just slow systems. It slows people. 

Planning stalls because nobody can predict how changes ripple. Estimates become fiction. Cross-team work turns into negotiation. Senior engineers become historians. New engineers drown in missing context. Teams avoid change because change feels dangerous.

Simplicity reverses this. When systems are understandable, planning becomes honest, work becomes collaborative, and people move quickly even when things go wrong.

## Simplicity Preserves Optionality

Teams talk about building for the future. Complexity destroys that future. Every extra component limits your ability to change direction. Every abstraction locks you into a pattern.

Simplicity keeps doors open. It allows redesign without unraveling everything. Optionality comes from clarity, not complexity.

## Patterns That Keep Systems Simple

**Surface area.** Keep it small. Every new module must prevent more complexity than it introduces.

**Defaults.** Prefer strong defaults over endless configuration. Every option is a decision someone will get wrong.

**Recovery.** Keep recovery paths short and predictable. If rollback requires a meeting, the system is too complex.

**Boundaries.** Maintain strict boundaries. Leaky abstractions become load-bearing confusion.

**Pruning.** Remove anything that no longer earns its place. Dead code is not neutral. It is camouflage for bugs.

**Root cause.** After incidents, fix the cause, not the symptoms. Workarounds are complexity waiting to compound.

These habits look unremarkable day to day. Over years they create systems that stay operable long after their authors have moved on.

## Simplicity and Capacity

Complexity drains capacity. People spend days unraveling behaviour that should not exist. Eventually this becomes culture. 

Nobody remembers what it felt like to move quickly.

Simplicity returns that capacity. It appears as fewer escalations, faster onboarding and clearer conversations. 

It is not elegance. It is protection from cognitive debt disguised as professionalism.

> Most best practices are simply the only way someone managed to make something work. They do not deserve the authority people give them.

## How Simplicity Enables Other Pillars

Simplicity makes every other pillar possible.

[**Consistency**](/articles/pillar_1_consistency/) stays consistent when there are fewer moving parts. Uniform behavior is easier to maintain when there is less behavior to maintain.

[**Resilience**](/articles/pillar_3_resilience/) improves when failure modes are predictable. Fewer edges mean fewer places for cascades to begin.

[**Maintainability**](/articles/pillar_4_maintainability/) becomes realistic when systems do not require heroics. Simple systems can be handed off without a month of knowledge transfer.

[**Transparency**](/articles/pillar_5_transparency/) follows naturally from obvious behavior. Systems that do what they appear to do need no interpretation.

[**Longevity**](/articles/pillar_6_longevity/) depends on systems that age without collapsing under their own weight. Simple architectures survive their original authors.

[**Standards**](/articles/pillar_7_standards/) are enforceable when surface area is small. Complexity creates exceptions. Simplicity eliminates them.

[**Trust**](/articles/pillar_8_trust/) grows when systems do not surprise people. Confidence comes from predictability, and predictability comes from simplicity.

Without simplicity, every other pillar becomes harder to achieve and easier to lose.

## The Essence of Simplicity

Simplicity is the discipline that prevents systems from turning on their creators. Every component becomes a long term relationship. If it cannot justify itself, it will punish you later.

Complexity pretends to offer power. What it offers is debt. It waits for the moment of maximum pressure and demands everything. That is why complex systems do not simply fail. They take half the company with them.

Simplicity is not modest engineering. It is survival engineering.

Refuse complexity now or answer to it forever.

---

**boring (adj.)**: The discipline of doing only what earns its keep. Every component must be understood, recoverable and operable without heroics.
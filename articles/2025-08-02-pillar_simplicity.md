---
title: "Pillar: Simplicity"
excerpt: "Simplicity removes everything that makes a system harder to understand, repair, and trust. If you can't sketch it on a napkin, it's too complex."
header:
  teaser: /assets/images/metronome.png
tags: [pillars, complexity, architecture]
layout: single
classes: wide
author: Dan Zrobok
date: 2025-08-02
---

Simplicity is the second pillar of BoringOps. Consistency gives you predictability. Simplicity gives you the ability to survive the moments where predictability collapses. Anyone who has been awake during a real incident knows this instinctively. They just never had the language for it.

Simplicity is not an aesthetic choice. It is not elegance for its own sake. It is the discipline of removing everything that makes a system harder to understand, harder to repair and harder to trust. A system can be powerful and still be simple. The things that make it complex are almost always the things nobody actually needed.

Most teams do not choose complexity outright. They drift into it. A small abstraction added for personal comfort. A temporary flag that quietly lives forever. A daily batch process that fixes a known bug in the database. Each decision feels harmless. The harm appears later when the architecture becomes something only a few people can navigate and nobody can explain without apologizing for it.

Simplicity is not austerity. It is refusing to let the system grow in ways that punish the people responsible for keeping it alive.

## The Real Source of Complexity

Complexity rarely comes from the demands of the product. It comes from human behaviour. Engineers want to be clever. Leaders want to appear modern. Teams want to avoid friction. Vendors want to sell you a future that depends on them. All of these motivations push in the same direction. They encourage architectures that look impressive and feel sophisticated while quietly eroding your ability to understand what you built.

But it doesn't feel dangerous at the time. Complexity often feels responsible. It feels like maturity. It feels like you are preparing for the future. In reality, you are building something fragile that only works as long as the exact conditions you imagined remain true.

Complexity is not usually created by malice. It is created by insecurity and optimism. That combination is far more dangerous.

## Complexity Is a Debt That Matures at Night

Complexity charges interest the moment it enters the system. You build it. You operate it. Eventually you must explain it to someone who was not there when it was created. That moment of explanation is where most architectures are revealed for what they are.

Complexity ages quickly. It turns into a collection of half remembered decisions that nobody wants to disturb. When the wrong person leaves, the architecture does not collapse immediately. It stalls. It becomes fragile in slow motion. Every deployment feels risky. Every incident turns into an archaeological dig. People stop touching the system because touching it feels unsafe.

Teams assume this is normal. It is not normal. It is accumulated cognitive debt that was never paid down.

## BoringOps Rejects Clever Architecture

Clever architecture fails where simple architecture survives. Clever solutions work beautifully in controlled environments. They fail in production where nothing stays controlled. The clever parts always rot first because they depend on assumptions that drift quietly over time. When they finally fail, they fail in ways that require heroic intervention.

If an architecture needs a long explanation to justify itself, it is not architecture. It is performance. Real systems must be legible. They must be understandable to someone who was not in the room when they were designed. If legibility is lost, reliability follows it out the door.

Simplicity is not basic. The opposite of clever is not primitive. It is clear. Advanced systems can still be simple when every part earns its keep and nothing exists for show. The core discipline is minimizing mutable state and enforcing strict boundaries keeping coupling low. Power does not require confusion.

Simplicity is not the absence of ideas. It is the refusal to build ideas that future operators will have to fight.

## The Bar Napkin Test

The napkin test reveals everything. If you cannot sketch the core of your system on a napkin and walk a new engineer through it in five minutes, the system is too complex. The napkin strips away the narrative. It exposes what is load bearing. It reveals where state actually lives. It shows how traffic really flows rather than how you wish it flowed.

If only one person can draw a napkin that matches reality, you do not have a system. You have a dependency on a single human being. That dependency is not resilience. It is fragility disguised as expertise.

Drama is not a sign of an exciting system. It is a sign that the system cannot protect its operators.

## A Real Story About Complexity Hiding in Plain Sight

> During an incident, a client once had an ESB that looked flawless. Logs green. Yet external service consumers kept receiving corrupted responses. Every team insisted their component was healthy. Hours later someone finally remembered a vendoe response cache sitting outside the network. It had a forgotten message size limit that silently truncated payloads. It existed only in production. Not staging. Not UAT.

This is complexity at work. It hides. It waits. And when it fails, everyone is certain the problem must be somewhere else.

## The Organizational Cost of Complexity

Complexity does not only damage systems. It damages organizations. Planning slows because nobody can reliably predict how changes will ripple. Estimates become fiction because nobody wants to admit they are guessing. Cross team work becomes negotiation instead of collaboration. Senior engineers become historians. New engineers become overwhelmed. Teams start avoiding change because change feels dangerous.

Simplicity restores momentum. It gives people the confidence to move quickly because the system is predictable even when things go wrong.

## Simplicity Is a Strategy for Optionality

Teams love to talk about building for the future. Complexity is the quickest way to lose that future. Every extra component limits your ability to change direction. Every abstraction ties you to a specific approach. Every unnecessary piece closes a future door.

Simplicity does the opposite. It keeps options open. It gives you the freedom to redesign parts of the system without untangling the entire structure. Simplicity turns architecture from something you are trapped inside into something you can evolve.

Optionality is not created through complexity. It is created through clarity.

## Patterns That Keep Systems Simple

Simplicity is a discipline, not a mood. The discipline looks like this.

- Keep the surface area small. 

Most teams proudly modularize themselves into a maze. The Single Responsibility Principle was never meant to justify unlimited sprawl. BoringOps adds a rule: every new module or service must prevent more complexity than it introduces.

- Prefer strong defaults rather than a menu of options.  
- Keep recovery paths short and predictable.  
- Use boundaries that are clear and strict.  
- Remove anything that no longer earns its place.

After incidents, address the surprise rather than wallpapering over it.

These habits look unremarkable in the moment. Over years, they create systems that stay understandable and operable long after the original authors have moved on.

## Simplicity and Capacity

Complexity quietly drains capacity. People spend entire days unraveling behaviour that should not exist. They assume the work is inherently difficult rather than recognizing the architecture has slowed them down. Over time this becomes the culture. Nobody remembers what it felt like to move quickly.

Simplicity returns that capacity. It shows up as fewer escalations, faster onboarding and clearer conversations. It shows up as a team with time to do real work instead of spending their energy explaining the past.

This is not about elegance. It is about protecting real people from cognitive debt disguised as professionalism.

> Most 'best practices' are simply the only way someone managed to make something work. They do not deserve the authority people give them.

## The Essence of Simplicity

Simplicity is the discipline that keeps a system from turning on its creators. Every component you allow in the architecture becomes a long-term relationship. If it cannot justify itself, it will punish you later.

Complexity pretends to offer power. What it really offers is debt. It waits until the worst possible moment and then demands everything at once. That is why complex systems do not simply fail. They take half the company with them.

Simplicity is not modest engineering. It is survival engineering.

Refuse complexity now or answer to it forever.

---

**boring (adj.)**: The discipline of doing only what earns its keep. Every component must be understood, recoverable and operable without heroics.

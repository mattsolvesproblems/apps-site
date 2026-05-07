---
title: Support
description: Support and contact info for the Praxis iOS app
---

# Praxis Support

Praxis is a habit and practice tracker for iOS, built by Matt Peterson. If something's broken, confusing, or you have an idea, this is where to start.

## The short version

Email **praxis.app.support@gmail.com**. I read every message.

## What you'll find here

- [Core concepts](#core-concepts) — practices, cadence, scoring, and how the app organizes your life
- [Flows](#flows) — chained practices that auto-advance through a routine
- [Links](#links) — scheduling constraints between practices
- [Lumen](#lumen) — the on-device AI that explains your patterns
- [Common questions](#common-questions) — quick answers to the things people ask most
- [Bugs and feedback](#bugs-and-feedback)
- [Refunds](#refunds)
- [Privacy](#privacy)

---

## Core concepts

A few ideas show up everywhere in Praxis. If you understand these, the rest of the app falls into place quickly.

### Practices

A **practice** is anything you want to track over time. A workout, a journal entry, watering the plants, calling your mom, twenty pages of a book. Praxis treats them all the same way: each one has a name, a place in your life, and a sense of how often you want to do it.

Add one from the **Practices** tab → tap **+**. Edit anything later by opening the practice and tapping **Edit**.

The vocabulary is deliberately broad. "Practice" comes from Aristotle's idea of *praxis* — purposeful action that becomes part of who you are when repeated. Whether you call them habits, rituals, chores, or routines, they're all practices in this sense.

### Cadence — target, min, and max

When you create a practice, Praxis asks how often you want to do it. You give it three numbers (in days):

- **Target frequency** — the rhythm you're aiming for. *"Run every 3 days."*
- **Minimum frequency** — the floor. Below this, the practice starts feeling overdue. *"Do it at least every 5 days."*
- **Maximum frequency** — the ceiling. Above this, it's been a long time. *"Even at the slowest, every 10 days."*

The three numbers create a band, not a single line. A practice doesn't have to land on its target every time to count as on-track. Life gets in the way; cadence accounts for that.

If you only want to set one number, just give Praxis the target — it'll fill in reasonable defaults for min and max.

### Scoring — good, neutral, overdue

Every practice gets a status based on when you last did it relative to its cadence:

- **Good** — within the target band. You're keeping rhythm.
- **Neutral** — past target but inside the min/max range. Still acceptable; do it soon.
- **Overdue** — past the maximum. The practice has slipped.

These show up as small colored indicators throughout the app: dots, bars, gradients, depending on the design style you're using. The **Minimal** style uses dot colors only. The **Aura** style washes the card background with status color. Pick whichever reads best to you under **Settings → Appearance**.

The scoring is decoupled from your overall progress score (in Stats) — being "neutral" or even "overdue" on one practice doesn't tank everything. It's just information about that one item.

### Areas, zones, and rooms

Most habit apps organize practices in a flat list. Praxis lets you give them a place — physically and metaphorically.

- **Zones** are top-level groupings. *Home, Workspace, Outdoors, Mental Health.*
- **Rooms and areas** sit inside zones. *Home → Kitchen, Bedroom. Mental Health → Reading, Meditation.*

You're not required to use this. A practice with no room or zone is fine — it just lives in "everywhere." But once you start grouping them, the app becomes much more useful: Focus shows urgency by zone, Plan helps you batch related work, Stats lets you see whether the **Yard** is keeping pace with **Home**.

The framing comes from a simple observation: your life has shape. The kitchen is different from the home office, and a Tuesday morning is different from a Saturday afternoon. Praxis lets you reflect that shape in how you track yourself.

### Insights — what Praxis notices

Praxis runs a set of pattern detectors over your completion history. Things like:

- *You're consistently faster at this than your estimate.*
- *You tend to do A and B in the same week.*
- *You haven't done this since Wednesday three weeks running — Wednesdays are slipping.*
- *Long sessions of this practice predict a longer gap before the next one.*

Insights appear in **Stats**, on the practice detail screen, and as the badge count on the **Lumen** menu item. They run entirely on-device — no servers involved. There are about twenty different pattern detectors, and they fire when there's enough data to be confident.

You can ask Lumen to explain any insight in more depth (see [Lumen](#lumen) below).

---

## Flows

A **Flow** is a chained sequence of practices that auto-advance.

Think of a morning routine. You meditate, then journal, then exercise. Each is a real practice you'd track on its own. With a Flow, you string them together: when you complete one, the next starts automatically. No tab-switching, no hunting through your list, no breaking concentration.

### How to set one up

Open the menu → **Flows** → **+**. Give the Flow a name (e.g., *Morning*). Add steps by picking practices from your library, in the order you want them. Save.

To run it, tap the Flow. The first practice opens with its timer ready. Complete it — log it normally — and the next one starts. The active Flow shows a banner at the top of Focus so you don't lose your place if you switch screens mid-routine.

### Why this is useful

Routines work because they remove decision friction. Once a sequence is established, you stop choosing what to do next; you just do the next thing. That's the whole point of a Flow.

A few examples of where they help:

- **Morning or evening rituals.** Wake-up sequence, wind-down sequence, anything anchored to a part of the day.
- **Sequential workout circuits.** Warm-up → main lift → cool-down, with timers built in.
- **Mise-en-place.** Setting up a workspace or kitchen before deeper work.
- **Multi-step chores.** Strip the bed → wash the sheets → remake. Each is a real practice; together they're a routine.

Flows aren't about doing more — they're about not having to think about how to start. The decision was already made when you built the Flow.

---

## Links

A **link** is a scheduling constraint between two practices. There are two kinds.

### Sequential links

*"Do A before B, within N days."*

Example: *Foam Roll → Run, within 1 day.* Praxis won't surface "Run" as a primary suggestion until "Foam Roll" has been done recently. If the link is broken, "Run" gets a small inline hint: *Do Foam Roll first.*

Use this when one practice meaningfully prepares for another. Stretching before running. Prepping a recipe before cooking it. Reading a chapter before discussing it.

### Spaced links

*"Wait at least N days between A and B."*

Example: *Heavy Cardio → Heavy Cardio, 2 days.* Praxis will block the second occurrence until enough time has passed.

Use this when two practices need recovery between them. Two leg workouts. Two long meditations. Two intense client sessions.

### Setting up a link

Open the practice that should depend on another. Inside the editor, scroll to **Links**. Add a link to the other practice, choose the type (sequential or spaced), and the window in days.

### Why this matters

Most habit apps treat practices as independent. They're not. Real life has dependencies: one thing makes another easier; some things shouldn't share a day. Links let Praxis know about those dependencies and respect them when it suggests what to do next.

You don't have to use links. Most practices don't need them. But when two practices clearly belong in a particular relationship, the app should know — and now it can.

---

## Lumen

**Lumen** is Praxis's on-device AI. It runs a small language model directly on your iPhone — no servers, no account, no data leaving your device.

You'll find Lumen in the side menu. Tap the flame.

### What Lumen is good at

Lumen's role is **explanation**, not data lookup. The app already knows your numbers — what's good, what's slipping, when you last did each practice. Lumen helps you make sense of those numbers in plain language.

The chip menu has five options:

- **Insights** — Pick a pattern Praxis has noticed (e.g., *consistency wins on Reading*) and Lumen explains what it means in your situation, with concrete suggestions.
- **Practice** — Pick a practice and Lumen reflects on how it's going. What's working, what's not, what to consider.
- **Recent** — A summary of what you've done lately. Deterministic, no AI involved — just a clean readout.
- **Slipping** — A list of practices that have fallen behind, ordered by urgency. Also deterministic.
- **Praxis** — Ask Lumen to explain the philosophy behind the app and the idea of practice itself.

### Why on-device

A few reasons:

1. **Your data never leaves your phone.** No "AI server" sees your habits, your reflections, your completion history. The model runs locally.
2. **It works offline.** On a plane, in a basement, with your wifi out — Lumen still works.
3. **No subscription.** The model is free once you've downloaded it. There's no recurring cost for AI features the way there is in most apps.

The trade-off is that the model is small (a few gigabytes) and not as fluent as a cloud-hosted GPT-4. It's accurate when explaining your data, but it's not a general-purpose chatbot. That's the deliberate design — Lumen is a coach for your practice, not a search engine.

### What Lumen can't do (yet)

- It doesn't have free-text chat in v1.0. The chip system covers the most useful 90% of what people want to ask, with much more reliable answers. Free chat returns in a future version once a larger on-device model becomes practical.
- It can't do calculations beyond what Praxis already computes. If you need a number, look in Stats — it's there.
- It can't browse the web, send messages, or do anything outside the app. It only sees what you've put into Praxis.

### Downloading the model

The first time you tap Lumen, you'll be asked to download the model. It's a one-time download (~2 GB) over wifi. After that, Lumen is always available offline.

---

## Common questions

### How do I back up my practices?

In the app: open the menu → Data & Storage → Export. You'll get a JSON file you can save to Files, email to yourself, or AirDrop.

To restore later: same menu → Import → pick the JSON file. Import replaces all current data, so back up first if you have anything you want to keep.

### What is Lumen, and where does it run?

Lumen is the on-device AI inside Praxis. It looks at your practice data and writes plain-language observations — what's holding, what's slipping, what works well together. It runs entirely on your phone. No servers, no account, no data sharing. See the [Privacy Policy](privacy) for the full picture.

### How do I unlock the full version?

Praxis is free to try, with all features available. After about two weeks of regular use, a one-time purchase ($9.99) keeps Praxis going for life — no subscription, no recurring charges. You'll see the unlock prompt in the app when you've crossed the threshold.

### How do I restore a previous purchase?

Open the menu → Settings → Restore Purchases. Make sure you're signed into the same Apple ID that bought Praxis originally.

### How do I change or turn off the daily notification?

Open the menu → Settings → Notifications. Toggle off, or change the time you want the daily check-in.

### How do I delete a practice or a logged session?

Practice: open the practice → Edit → Delete. Logged session: open Stats → tap the session card → delete.

## Common workflows

A few patterns that come up over and over. Each is a way to get more out of features Praxis already has.

### Build a morning routine

1. Add the individual practices first — *Meditate, Journal, Workout, Shower* — each as its own practice.
2. Open the menu → **Flows** → **+**.
3. Name the Flow *Morning*. Add the practices in order. Save.
4. Tap the Flow tomorrow morning. Each practice flows into the next, no decisions in between.

The reason this works better than a single "Morning Routine" practice: you still get separate cadence, scoring, and history for each piece. *Workout* is on its own three-day cycle whether or not you did the rest of the routine that day.

### Track something that doesn't fit a fixed schedule

Some practices aren't daily or weekly — they're "when it makes sense." *Call Mom. Deep clean the bathroom. Read fiction.*

Set the **target** to roughly how often you'd like to (every 7 days, every 14, every 30) and **max** to your patience level (when does it start to feel neglected?). Don't worry about getting it exact. Adjust the numbers later if scoring doesn't match how you actually feel about the practice.

### Pair related practices with a link

Some pairs naturally belong together — one prepares for the other, or two of them shouldn't share a day. Open the practice that should depend on another, scroll to **Links**, add the link.

Common ones:
- *Stretch → Run, within 1 day.*
- *Cardio → Cardio, 2 days minimum.*
- *Plan the week → Execute the week, within 1 day.*

Most practices don't need a link. Use them when the dependency is obvious.

### Understand what's slipping

Open Lumen → tap **Slipping**. You'll get a list of practices that are past their max, ordered by how overdue they are. No AI involved — just a clean readout from the rule-based scoring.

If you want to know *why* a particular practice is slipping (was it always this way, or did it change recently?), tap that practice in Stats and look at the cadence chart. The pattern is usually obvious once you can see the timeline.

### Plan a realistic week

Open the **Plan** tab. Praxis suggests practices for each day of the upcoming week based on cadence and what's overdue. If two linked practices land on the same day in a way that violates a constraint, the app shows a swap indicator so you can rebalance.

Plan is most useful when you've got 10+ practices going. With fewer than that, Focus alone is usually enough.

---

## Bugs and feedback

If something doesn't work right, or you have an idea for what Praxis should do better, email **praxis.app.support@gmail.com**. Include:

- What you were trying to do
- What happened instead
- Your iOS version and device model (Settings → General → About)

Screenshots help.

## Refunds

Refunds for the Praxis in-app purchase are handled by Apple, not by me. Open the [Apple "Report a Problem"](https://reportaproblem.apple.com/) page, sign in, find Praxis in your purchase history, and request a refund. Apple makes the decision — I don't have visibility into individual transactions.

## Privacy

See the full [Privacy Policy](privacy) for details on what Praxis stores and where. Short version: nothing leaves your phone unless you explicitly export it.

## Contact

For anything I haven't covered here, email **praxis.app.support@gmail.com**.

— Matt Peterson

---
name: startup-playbook-skill
version: 1.0.0
description: A step-by-step operating playbook for building a high-growth startup, distilled from Y Combinator's "How to Start a Startup" (CS183B) lectures. Use it to figure out what stage a founder is at and what to do next.
triggers:
  - how do I start a startup
  - build a startup step by step
  - startup playbook
  - what should I do next in my startup
  - is my startup idea good
  - how do I get my first users
  - do I have product market fit
  - how do I raise money for my startup
  - review my startup pitch
  - help me build my startup
allowed-tools:
  - Read
  - Write
  - Edit
  - WebSearch
  - AskUserQuestion
---

# Startup Playbook

A stage-by-stage guide to building a startup whose goal is **hyper-growth and a large, durable company**. Distilled from YC's *How to Start a Startup* (Stanford CS183B): Altman, Graham, Thiel, Moskovitz, Cheung, Schultz, Hale, Chesky, the Collisons, Silbermann, Levie, Hoffman, Rabois, Horowitz, Shear, Rahman, Andreessen, Conway, Bosmeny, and others.

> This advice is for growth startups. Much of it is wrong for a small business, a consultancy, or a big company. Warn the user if their goal isn't a large, fast-growing company.

## How to use this skill

1. **Locate the founder's stage.** Ask 2–4 quick questions if it isn't obvious: Do you have an idea you're compelled by? A cofounder? A shipped product? Users? Are they retaining? Revenue? Are you raising? Map the answer to a stage below.
2. **Work the *current* stage — don't skip ahead.** The single most common failure is doing a later stage's work early: optimizing growth before retention, hiring before you must, fundraising before traction, adding process before product/market fit. If the user asks about a later stage, answer, but flag what they should finish first.
3. **Load the matching reference file** in `references/` for depth before giving detailed advice. Each file is self-contained and cites the lecture(s) it comes from.
4. **Use the gates.** Each stage has an exit gate — a concrete signal that they're ready to advance. If the gate isn't met, the work is to meet it, not to move on.
5. **Give a recommendation, then the next 1–3 concrete actions.** Founders are drowning in options; your job is to narrow, not to survey. Be direct.
6. When reviewing their pitch, idea, retention, or hiring plan, apply the specific checklists in the reference files rather than generic advice.

## The two invariants (true at every stage)

- **Before product/market fit, only two things matter: build the product and talk to users.** Almost everything else (PR, conferences, partnerships, recruiting advisers, fancy offices, elaborate process) is a distraction. Be suspicious if the founder's time isn't mostly on those two.
- **Execution and momentum are the lifeblood.** Ideas are ~1/100th of the work; there's no credit for trying, only for making something the market wants. Growth/momentum must never be lost focus of. Manage your own psychology — the final cause of death for most startups is the founders giving up.

## The stages

| # | Stage | Exit gate → advance when… | Reference |
|---|-------|---------------------------|-----------|
| 0 | **Mindset & readiness** — should you even do this? | You "can't not do it" and are ready for a ~10-year commitment | `00-founder-mindset.md` |
| 1 | **Idea & market** — pick something worth 10 years | A clear, mission-driven idea; a small market you can monopolize that grows huge; a real "why now" | `01-idea-and-market.md` |
| 2 | **Cofounders** — get the founding team right | 2–3 cofounders you've known/worked with, near-equal equity, vesting signed | `02-cofounders.md` |
| 3 | **Talk to users** — become the expert | You know the target user, their real problem (one sentence), and have interviewed the right people | `03-talk-to-users.md` |
| 4 | **Build the product** — make something users *love* | A simple MVP a small number of users love; a tight feedback loop | `04-build-product.md` |
| 5 | **Launch & first users** — do things that don't scale | First users recruited by hand; some are "champions" who tell others | `05-launch-and-first-users.md` |
| 6 | **PMF & growth** — retention first, then scale channels | A cohort retention curve that flattens above zero; a north-star metric; a working channel | `06-pmf-and-growth.md` |
| 7 | **Fundraising & sales** — get money and revenue | Traction that lets you raise from strength; repeatable early sales | `07-fundraising-and-sales.md` |
| 8 | **Hiring, culture & management** — build the org | First hires are near-founders; written values; you manage as an "editor" | `08-hiring-culture-management.md` |
| 9 | **Legal, finance & scaling** — build a great *company* | Clean cap table & docs; management structure; repeatable innovation | `09-legal-and-scaling.md` |

Stages 0–6 are strictly sequential-ish; 7–9 run in parallel with the later stages and recur. Cofounders (2) and talking to users (3) never stop.

## Fast diagnostics (jump straight to the real problem)

- **"Is my idea good?"** → Stage 1. Check: mission you'd give 10 years to; a *small* market you can dominate then expand; market *growth rate* > current size; a crisp "why now"; sounds slightly bad-but-actually-good; you'd build it because you need it. `01-idea-and-market.md`
- **"How do I get users / no one is signing up?"** → Stage 5. Recruit the first ones by hand; do unscalable things; talk to them constantly. `05-launch-and-first-users.md`
- **"We're not growing."** → First check *retention*, not acquisition. No flat retention curve = no PMF; fix the product, don't buy growth. `06-pmf-and-growth.md`
- **"Should we raise money?"** → Only from strength (traction, or a plan to grow without it). Raising is not success; it's the easiest hard thing you'll do. `07-fundraising-and-sales.md`
- **"Cofounder tension / equity split."** → Set it near-equal, early, with vesting. This is the #1 early killer. `02-cofounders.md`
- **"When do I hire?"** → Try not to. A single mediocre early hire can kill the company. `02-cofounders.md` + `08-hiring-culture-management.md`
- **"How do I decide X as CEO?"** → See the decision through the eyes of the *whole* company, not just the person in the room. `08-hiring-culture-management.md`

## Operating principles to repeat back to founders

- Make something a **small number of users love** > a large number who merely like it. Word-of-mouth growth is the signal it's working.
- Start **simple** and do one thing extremely well. Be fanatical about details and support.
- **Aim for monopoly, avoid competition** (Thiel). Win a small market completely, then expand in concentric circles. Be the *last* mover, not the first.
- **Retention is the #1 driver of growth** (Schultz). Don't do growth tactics without PMF.
- **Marketing/sales is a tax you pay for not making the product remarkable** (Hale). Reduce churn — it's cheaper than raising conversion.
- **Focus:** pick the 2–3 things that matter; say no ~97/100. **Intensity:** outwork competitors by a little; move fast *and* obsess over quality.
- Hire people who are **smart, get things done, and you want to be around**; work with them before committing. Fire fast when it's consistently not working.
- **"Be so good they can't ignore you"** (Steve Martin, via Andreessen) — improving the business beats improving the pitch.
- The journey is long: expect a "trough of sorrow" — often ~1,000 days before the graph turns up (Airbnb). Keep momentum with small wins.

Now identify the stage and open the matching reference file.

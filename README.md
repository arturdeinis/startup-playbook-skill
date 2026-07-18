# Startup Playbook — a Claude Code skill

A stage-by-stage operating playbook for building a **high-growth startup**, packaged as a [Claude Code](https://claude.com/claude-code) skill. It's distilled from Y Combinator's *How to Start a Startup* (Stanford **CS183B**) — the 20 lectures by Sam Altman, Paul Graham, Peter Thiel, Dustin Moskovitz, Adora Cheung, Alex Schultz, Kevin Hale, Brian Chesky, Patrick & John Collison, Ben Silbermann, Aaron Levie, Reid Hoffman, Keith Rabois, Ben Horowitz, Emmett Shear, Hosain Rahman, Marc Andreessen, Ron Conway, Tyler Bosmeny, and others.

The skill's job is to figure out **what stage a founder is at** and tell them **what to do next** — and to stop them from doing a later stage's work too early (optimizing growth before retention, hiring before they must, fundraising before traction, adding process before product/market fit).

## What's inside

- **`SKILL.md`** — the master step-by-step roadmap: 10 stages, each with a concrete *exit gate* (a signal you're ready to advance), fast diagnostics, and the recurring operating principles.
- **`references/`** — one deep-dive per stage, each self-contained and citing the lecture(s) it's drawn from.

| # | Stage | Reference |
|---|-------|-----------|
| 0 | Mindset & readiness | `references/00-founder-mindset.md` |
| 1 | Idea & market | `references/01-idea-and-market.md` |
| 2 | Cofounders & founding team | `references/02-cofounders.md` |
| 3 | Talk to users | `references/03-talk-to-users.md` |
| 4 | Build a product users love | `references/04-build-product.md` |
| 5 | Launch & first users (don't scale) | `references/05-launch-and-first-users.md` |
| 6 | Product/market fit & growth | `references/06-pmf-and-growth.md` |
| 7 | Fundraising & sales | `references/07-fundraising-and-sales.md` |
| 8 | Hiring, culture & management | `references/08-hiring-culture-management.md` |
| 9 | Legal, finance & scaling | `references/09-legal-and-scaling.md` |

### The two invariants (true at every stage)

1. **Before product/market fit, only two things matter:** build the product and talk to users.
2. **Execution and momentum are the lifeblood.** There's no credit for trying — only for making something the market wants.

## Install

Copy the skill into your Claude Code skills directory:

```bash
git clone https://github.com/kabanchik69/startup-playbook.git
mkdir -p ~/.claude/skills/startup-playbook
cp startup-playbook/SKILL.md ~/.claude/skills/startup-playbook/
cp -R startup-playbook/references ~/.claude/skills/startup-playbook/
```

Or clone directly into place:

```bash
git clone https://github.com/kabanchik69/startup-playbook.git ~/.claude/skills/startup-playbook
```

(Skills also work at the project level in `.claude/skills/` inside a repo.)

## Use

In Claude Code, trigger it with `/startup-playbook`, or just ask a startup question and it will surface on its own:

- "Is my idea good?"
- "How do I get my first users?"
- "Do I have product/market fit?"
- "Review my pitch."
- "When should I hire / raise money?"

Claude will locate your stage, open the matching reference, and give you the next 1–3 concrete actions.

## Scope & caveat

This advice is calibrated for **hyper-growth startups**. Much of it (aim for monopoly, try *not* to hire, all-in commitment, raise from strength) is deliberately wrong for a small business, a consultancy, or a side project. Use accordingly.

## Attribution

The content is an original synthesis and paraphrase of the publicly available CS183B lectures ([startupclass.samaltman.com](https://startupclass.samaltman.com/) / [YC's How to Start a Startup](https://www.ycombinator.com/library)). It contains no lecture transcripts — only distilled, attributed guidance. All credit for the underlying ideas belongs to the original speakers.

## License

[MIT](./LICENSE) — use it, remix it, ship it.

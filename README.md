# Startup Playbook skill

A stage-by-stage operating playbook for building a **high-growth startup**, distilled from Y Combinator's *How to Start a Startup* (Stanford **CS183B**) — the 20 lectures by Sam Altman, Paul Graham, Peter Thiel, Dustin Moskovitz, Adora Cheung, Alex Schultz, Kevin Hale, Brian Chesky, Patrick & John Collison, Ben Silbermann, Aaron Levie, Reid Hoffman, Keith Rabois, Ben Horowitz, Emmett Shear, Hosain Rahman, Marc Andreessen, Ron Conway, Tyler Bosmeny, and others.

It's just plain Markdown — a master `SKILL.md` roadmap plus per-stage references — so it's **not tied to any one tool.** Read it yourself, drop it into any AI assistant or agent, or install it as an agent skill. Its job is to figure out **what stage a founder is at** and tell them **what to do next** — and to stop them doing a later stage's work too early (optimizing growth before retention, hiring before they must, fundraising before traction, adding process before product/market fit).

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

## How to use it

The whole thing is portable Markdown, so use whichever mode fits.

### 1 · Read it (no tools)

Open `SKILL.md`, find your stage, then read the matching file in `references/`. It's written to be read by a person as much as by a machine.

### 2 · With any AI assistant or agent

Model-agnostic — works with ChatGPT, Claude, Gemini, Cursor, Copilot, or any LLM / agent framework. Give the assistant `SKILL.md` (and the relevant `references/*.md`) as context — a system prompt, custom instructions, an uploaded file, or a pasted block — then ask your question:

> *Use this playbook. Figure out what stage my startup is at and tell me what to do next.* — then attach or paste `SKILL.md`.

### 3 · As a Claude Code skill

Clone it into your skills directory:

```bash
git clone https://github.com/arturdeinis/startup-playbook-skill.git ~/.claude/skills/startup-playbook-skill
```

(Skills also work per-project in a repo's `.claude/skills/`.) Then invoke it with `/startup-playbook-skill`, or just ask a startup question and it surfaces on its own — "Is my idea good?", "How do I get my first users?", "Do I have product/market fit?", "Review my pitch", "When should I hire / raise money?" Claude locates your stage, opens the matching reference, and gives you the next 1–3 concrete actions.

**Triggering is semantic, not keyword-exact.** Claude reads the skill's name and description and decides whether your request is about building a high-growth startup — it doesn't scan for a fixed word list. So the examples above (and the `triggers` in `SKILL.md`) are illustrative, not an allowlist: an intent-matching request fires it even with no shared words ("my users keep churning, what do I do?"), a passing mention of "startup" won't, and lifestyle-business / consultancy / side-project questions may not match at all. To widen or narrow it, edit the `description` and `triggers` in `SKILL.md`.

## Scope & caveat

This advice is calibrated for **hyper-growth startups**. Much of it (aim for monopoly, try *not* to hire, all-in commitment, raise from strength) is deliberately wrong for a small business, a consultancy, or a side project. Use accordingly.

## Attribution

The content is an original synthesis and paraphrase of the publicly available CS183B lectures ([startupclass.samaltman.com](https://startupclass.samaltman.com/) / [YC's How to Start a Startup](https://www.ycombinator.com/library)). It contains no lecture transcripts — only distilled, attributed guidance. All credit for the underlying ideas belongs to the original speakers.

> **Unofficial project.** This is an independent, fan-made summary. It is **not affiliated with, sponsored by, or endorsed by** Y Combinator, Stanford, or any of the lecturers. "Y Combinator," "How to Start a Startup," and the speakers' names are used only to attribute the source material.

## License

[MIT](./LICENSE) — use it, remix it, ship it.

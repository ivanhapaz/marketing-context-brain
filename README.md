# Context Brain

**Building a marketing agent? Build its brain first.**

The fastest way to build a good AI marketer is to not automate it yet. Give it enough context to have real marketing judgment, prove that judgment somewhere cheap, and only then wire it into a stack.

This is a Claude skill for the first part. Install it, tell it what kind of marketing brain you're building, and it goes to work: pulling your data, researching your category, drafting real artifacts, arguing with you about what it found, and assembling the whole thing into markdown you own.

It doesn't hand you blank templates. It does the homework and asks you for the judgment.

## What you end up with

Eleven interlocking documents:

| # | Document | Job |
|---|---|---|
| 01 | Spine | Master context and routing. Wins conflicts. |
| 02 | Market & Category Research | Category dynamics, alternatives, buyer context, material constraints. |
| 03 | Competitor Reference | Fast positioning guidance during active work. |
| 04 | Customer & Performance Evidence | Patterns from customers, users, product usage, sales, campaigns. |
| 05 | ICP | Segments, triggers, jobs, objections, proof. |
| 06 | Voice & Tone | Testable language principles and a real variant kit. |
| 07 | Design System | Brand guidance translated into rules an agent can execute. |
| 08 | Brand Asset Index | Every usable asset mapped and described in text. |
| 09 | Workflow | The operating loop, permissions, and approval gates. |
| 10 | Instructions | Lean role, routing, precedence, hard rules. |
| 11 | Decision Log | Every hard rule, the mistake behind it, and when it expires. |

The number isn't sacred. The architecture is: evidence before synthesis, depth docs plus fast references, explicit precedence, and an operating layer that travels with the knowledge.

## How the work actually goes

**AI investigates. The marketer decides.**

Claude pulls what it can reach, reads what you already have, and comes back with a draft and a point of view. You correct the judgment — the taste, the limits, the things that cost you money to learn. Nobody fills in a blank form. Where you disagree, it says so with evidence, once, and then takes your call.

Uncertainty stays marked instead of quietly hardening into fact. Hard rules get recorded with their reasons, so a year from now you know which ones have expired.

## Install it

**Claude.ai** — download this repo as a ZIP, upload it as a custom skill, then say:

> Help me build a context brain.

**Claude Code** — drop the `context-brain` folder in `~/.claude/skills/` (personal) or `.claude/skills/` (project).

**No skills, don't care** — put the files in a Claude Project and tell Claude to follow `SKILL.md`. It's all plain markdown. Works fine.

## What good looks like

The hardest part to describe in prose is the level of specificity that makes these docs work. So there are worked excerpts in [`assets/examples.md`](assets/examples.md) — a real testable voice principle with its pass/fail lines, one segment that changes the marketing sitting next to one decorative persona, and a decision log entry with the field everyone skips. All from a fictional company. Read them for shape, not content.

## How you know it worked

Not by word count, and not because all eleven files exist.

Give it a real task it's never seen and see whether the output is something you'd have approved anyway. There are eight acceptance tests in [`references/evaluation.md`](references/evaluation.md) — new campaign brief, ten genuinely different concepts, a claim it should refuse, a gate it shouldn't walk through. When it fails, fix the brain, not the prompt.

## The eleventh document

The Decision Log didn't exist in the build this method came from. It got reconstructed later, painfully, by reading the brain's own prohibition language and reverse-engineering what must have gone wrong to produce each rule.

Every hard rule in a mature brain is a fossilized mistake. Six months on, everyone remembers the rule and nobody remembers why. So doc 11 is the thing I'd do differently: write it while it's cheap. When you catch yourself typing "never," stop and log why.

The rest is what actually worked, scars included — including the expensive one, which is in [`references/principles.md`](references/principles.md): live data went in last, falsified a premise the spine had already spread into three docs, and cost four fixes. The method puts it first so yours doesn't.

## Same brain, different body

It's markdown, not a prompt trapped in a product. Test the judgment in a chat window today; move the same files into a more autonomous stack when they hold. The implementation changes. The accumulated judgment travels.

## Provenance

Built by [Ivanha Paz](https://www.linkedin.com/in/ivanha-paz) from a working system: the in-house Meta ads marketer for a real lead-gen program, currently living in a Claude Project, on its way to a production stack.

If you build one, tell me what you learn.

## License

MIT. Take it, fork it, make it yours.

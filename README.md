# Context Brain

**A method for building the context an AI marketer actually needs.**

Ten interlocking docs (plus an eleventh most people skip) that give an agent enough context to do real marketing work. Plain markdown. Prototype them in a chat window, then move the same files into whatever stack runs the work for real.

The premise: AI output is generic when you starve it of context. This is a method for producing that context cheaply, and putting it where an agent can use it.

## What this actually does

It's an interviewer, not a template pack. Load it, tell Claude you want to build a context brain, and it asks you questions — what's the product, what data can you connect, who's actually bought, what would you never say in an ad — then writes the docs with you, in the right order, and pushes back when an answer is a vibe instead of a rule.

The order matters more than the docs. Live data first, then extraction, then derivation, then synthesis. There's a reason for that, and it's in `references/principles.md`.

## The docs it builds

| # | Doc | Job |
|---|---|---|
| 01 | Spine | Master context. Wins ties. |
| 02 | Market Research | The category, the competitors, the regulator, the fear. |
| 03 | Competitor Reference | The fast companion. Positioning calls mid-task. |
| 04 | Buyer & Sales Data | Who actually bought, as anonymized patterns. |
| 05 | ICP | Segments the data supports, with objections and counters. |
| 06 | Voice & Tone | Testable principles, banned words, a variant kit. |
| 07 | Design System | The brand guide, translated into executable rules. |
| 08 | Brand Asset Index | Every real file, mapped and described in words. |
| 09 | Workflow | The loop, and where a human says yes. |
| 10 | Instructions | Lean. Role, hard rules, routing. |
| 11 | Decision Log | Every "never," and the mistake that caused it. |

## How to use it

**In claude.ai:** download this repo as a zip, then Settings → upload it as a custom skill. Say "help me build a context brain" and it starts.

**In Claude Code:** drop the `context-brain` folder into `~/.claude/skills/` (personal) or `.claude/skills/` (project).

**Without skills, in any chat:** open `references/doc-specs.md` and `references/interview.md`, paste them into a Claude Project or a chat, and say *"interview me and build these docs with me, one at a time."* Works fine.

## The honest caveat

Doc 11 — the decision log — doesn't exist in the build this method came from. It was reconstructed afterward, painfully, by reading the brain's own prohibition language and reverse-engineering what must have gone wrong to produce each rule.

Every hard rule in a mature brain is a fossilized mistake, and six months later nobody remembers which mistake. So doc 11 is here as the thing I'd do differently: write it while it's cheap. When you catch yourself typing "never," stop and log why.

The rest of the method is what actually worked, scars included. `references/principles.md` names the mistakes, including the expensive one — live data went in last, falsified a premise the spine had already propagated into three docs, and cost four fixes. This method puts it first so yours doesn't.

## Provenance

Built by [Ivanha Paz](https://www.linkedin.com/in/ivanha-paz), from a working system: the in-house Meta ads marketer for a real ad program, currently running as a Claude Project, moving to a production agent stack.

If you build one, tell me what you learn.

## License

MIT. Take it, fork it, make it yours.

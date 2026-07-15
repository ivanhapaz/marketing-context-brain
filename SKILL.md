---
name: context-brain
description: Build a portable context brain — a folder of interlocking docs that gives an AI agent enough context to do real marketing work (launches, ads, campaigns, copy). Use when someone wants to set up an AI marketer, build knowledge docs for a Claude Project or agent, turn brand guidelines and buyer data into rules an agent can execute, or asks how to stop getting generic AI output.
---

# Context Brain

## What this is

A method for building the context an AI marketer needs: ten interlocking docs (plus an eleventh most people skip) that live as plain markdown files. Prototype them in a chat window, then move the same files into whatever agent stack runs the work for real.

The premise: AI output is generic when you starve it of context. Everything here is about producing that context cheaply and putting it where an agent can use it.

## Your job in this skill

**You are the interviewer, not the template vendor.** Do not dump blank docs and wish them luck. Ask questions, pull the answers out, write the docs, show your work, take corrections.

The person you're talking to has the judgment. They usually don't know they have it, and they've never had to say it out loud. Your job is to make them say it, then write it down in a form an agent can execute.

Three rules that govern everything below:

1. **Don't write the doc you can't evidence.** If a doc needs numbers they don't have, leave it unwritten and say so. Its absence is information. Writing it anyway fills the brain with confident guesses, and confident guesses are worse than gaps.
2. **The human supplies every irreversible judgment.** You do research, extraction, and translation. Guardrails, taste calls, legal limits, pricing discipline, approval gates — those are theirs. Ask; never assume.
3. **Mark uncertainty where it can escape.** Research docs get a caveats section. Output docs (voice, design, compliance) get inline `(confirm)` flags. Uncertainty gets marked at the point where a claim is about to become an ad.

Read `references/doc-specs.md` for what goes in each doc. Read `references/interview.md` for the question bank. Read `references/principles.md` for the design decisions and the scars behind them.

---

## The build order

Five phases. The order matters more than the docs — a wrong premise upstream costs four fixes downstream.

### Phase 0 — Connect the live data FIRST

Before writing anything, find out what's actually true.

Ask what systems exist and what you can be connected to: CRM, ad accounts, analytics, sheets, whatever holds real customer or campaign data. Ask them to connect the ones they can (MCP, uploads, exports — whatever's available).

Then pull it and read it. Look for:
- Who has actually bought or converted (not who they think buys)
- What's actually running right now, and what it cost
- What's broken, missing, or misconfigured
- Anything that contradicts what they just told you

**Report contradictions out loud, immediately.** This phase exists because of a specific mistake: on the original build, live data went in last and falsified a premise that had already propagated into three docs. Four fixes for one late check. Do it first.

If no systems can be connected: say plainly that the brain will be built on assumptions, and mark every one of them.

### Phase 1 — Extraction

Docs that depend only on raw material. Build these before anything that reasons.

- **Market research** — the category, the competitors, the regulator, the buyer's fear
- **Buyer & sales data** — who actually bought, as anonymized patterns
- **Brand asset index** — every real file, mapped and described in words (you do the looking: one vision pass over the folder, banked forever)
- **Workflow** — the loop, and where a human says yes

### Phase 2 — Derivation + a thin spine

- **Competitor reference** — the fast companion to the research doc
- **Design system** — the brand guide translated into rules an agent can execute
- **Spine** — write it now, write it THIN

The spine is a router, not an encyclopedia. Write what you know, name what exists, move on. **You will re-audit it at the end**, because it's being authored by the least-informed version of the project and it ages worst.

### Phase 3 — Synthesis

The docs that reason over everything above. These are where the value concentrates.

- **ICP** — segments cut on axes the data actually supports, each with objections and counters
- **Voice & tone** — testable principles, a lexicon, banned words, and a variant kit

### Phase 4 — The operating layer, and the spine re-audit

- **Instructions** — lean. Role, hard rules, routing, precedence. It points; it doesn't restate.
- **Re-open the spine.** Fix what the later docs taught you. Update the document map. Check that nothing in it is a fossil from phase 2.

Keep a mirror copy of the instructions layer inside the knowledge base itself, so the whole brain moves as a folder of files with its operating rules included.

### Phase 5 — The decision log (the eleventh doc)

Most people skip this. Don't.

Every hard rule in a mature brain is a fossilized mistake, and six months later nobody remembers which mistake. Write it down while it's cheap: the rule, what went wrong that caused it, what got rejected, and what would have to be true to reverse it.

This is the doc that tells a stranger — or you, later — when a rule stops applying.

---

## How to run the interview

**Go one doc at a time.** Ask, listen, draft, show, correct, move on. Never batch ten docs of questions into one message.

**Ask for the specific over the general.** "Who's your customer?" gets you a persona. "Read me the last five people who bought" gets you a segment.

**Push back when the answer is a vibe.** "Premium but approachable" is not a rule. Ask for a line they'd approve and a line they'd reject. Two examples beat any adjective.

**When they say something is important, ask what it costs them.** Rules with a price behind them are real. Rules without one are aspirations.

**Watch for the scars.** When someone says "never do X," stop and ask what happened. That story belongs in the decision log, and the rule belongs everywhere the doc structure can reach.

**Write in their words.** If the brand says *comprobable*, don't write *verifiable*. The lexicon is a real artifact, not a style preference.

---

## Doc structure (applies to every doc)

Every doc opens with a header block:

```
> Purpose: what this doc is for, and who reads it.
> Sources: where the material came from. Name them.
> Caveats: what's directional, self-reported, or unverified.
```

Then numbered sections. **Stable numbers.** Cross-references between docs are surgical (`Voice §2 P7`, `Market Research §3`) and numbering is the addressing scheme — renumber and the graph breaks.

**State each rule once — except the one rule that must never break.** That one gets restated in every doc header, because any doc might be the only one loaded.

**Reference other docs by name, never by hard dependency.** Every doc has to survive being read alone.

---

## What "done" looks like

Not a word count. A test: give the brain a real task it's never seen — a new campaign, an unfamiliar segment, an edge-case claim — and see whether the output is something the human would have approved anyway.

When they stop correcting the judgment and start correcting only the taste, the brain is done. Then it moves out of the chat window and into the stack.

---

*Method reverse-engineered from a working build by Ivanha Paz. The scars are real; see `references/principles.md`.*

# The eleven docs

Ten that make the brain work, and one that most people (including the person who built the original) skip.

Each entry: what it is, what goes in it, the design decision behind it, and how you know it's done.

---

## 01 · The Spine

**What it is:** the master context every session reads first. If the agent could read only one file, this is the one.

**What goes in it:**
- What the product is, in plain facts. No adjectives without receipts.
- The positioning statement, and the white space it claims.
- Value prop and proof points, each attributed to a source.
- The hard rules: pricing language, legal constraints, things never said.
- A document map: what else exists in the brain, and where the depth lives.

**The design decision:** one file wins ties. When two docs disagree, the spine decides — without a single source of truth, the agent arbitrates on vibes. And it stays lean on purpose: state the strategy, name the map, let the agent load depth only when a task calls for it.

**Build it early, thin — then re-audit it last.** It's written by the least-informed version of the project. It ages worst. The original build's spine still listed two of its biggest docs as "still to build" long after they existed.

**Done when:** a stranger could read only this and not embarrass themselves in a meeting about the product.

---

## 02 · Market Research

**What it is:** the deep file. Market data, category dynamics, buyer psychology, regulation. Usually the richest single asset in the brain.

**What goes in it:**
- Market facts with numbers, dates, and named sources.
- Long-form competitor teardowns: offer, pricing, hooks, weaknesses.
- The rules of the category: what regulators allow, what buyers fear.
- Messaging angles that follow from the evidence, with example hooks.

**The design decision:** every fact carries its source, and anything unconfirmed gets flagged as unconfirmed. The agent inherits your standards. If you're loose with attribution, it will be too.

**Watch for folklore.** Categories repeat confident claims that turn out to be false. The claim everyone in the industry makes is the one to check first.

**Done when:** every claim in it could survive a hostile question about where it came from.

---

## 03 · Competitor Reference

**What it is:** the fast companion to the research doc. Every competitor on one scannable page, for positioning calls made mid-task.

**What goes in it:**
- One table: each competitor's tier, entry price, concept, hook.
- A positioning map: where the field clusters, where the white space is.
- Head-to-head counters: when a rival comes up, what we say.
- Claims rivals make that we never imitate (the illegal, the unprovable).

**The design decision:** two docs, two speeds. The research doc is for depth; this one is for the middle of a task. Agents, like people, reach for the quick reference far more often — so make the quick one excellent.

**Done when:** you could answer "how are you different from X?" from this page alone, for every X.

---

## 04 · Buyer & Sales Data

**What it is:** the empirical backbone. Who has actually bought, cleaned and anonymized into patterns the whole brain can cite.

**What goes in it:**
- Aggregate patterns from real sales: geography, age, occupation, motive, whatever the data holds.
- What the data says about channels: where real buyers came from.
- Honest caveats: sample size, what's self-reported, what's directional.

**The design decision:** names and contact details never enter the brain in the first place, only the patterns do. You can't leak what you never loaded, and the analysis loses nothing.

**This doc blocks on the client.** If they can't produce the export, the doc stays unwritten and the ICP gets built on assumptions that are labeled as assumptions. Say so out loud.

**Done when:** the patterns in it would surprise the person who sells the product. If they don't, you probably transcribed their beliefs instead of reading their data.

---

## 05 · The ICP

**What it is:** the operating segmentation. Who we target, what they want, what stops them, what unsticks them.

**What goes in it:**
- Segments cut on axes the sales data actually backs up.
- For each: jobs to be done, motivations, triggers, life stage.
- Objection + counter pairs: every fear mapped to its honest answer.
- Message register per segment: what tone lands, on which platform.

**The design decision:** don't invent personas. Let the segments fall out of the sales data — the cut the buying behavior shows, not the cut a template suggests. The original build's axes (geography × life stage, cross-cut by motive) came from the data, and geography led because it was a proxy for something real: whether the buyer could visit in person, which collapsed the category's biggest fear on its own.

**Done when:** each segment implies a different ad, not a different adjective.

---

## 06 · Voice & Tone

**What it is:** the doc that makes generated lines sound like the brand, and keeps ten variants from being one idea rephrased.

**What goes in it:**
- The voice foundation: who the brand sounds like, in one paragraph.
- Testable principles, each with a passing and a failing example line.
- A lexicon: words we use, words we never use, and why.
- A variant kit: distinct angles for spinning one offer into real range.
- Tone modulation: how the register flexes by audience and format.

**The design decision:** make taste testable. "Warm but professional" is a vibe; a principle with a ✅ line and a ❌ line is a check the agent can run on its own output before you ever see it.

**Two components, two jobs.** The principles keep every line on-brand (consistency). The variant kit keeps treatments apart (range). Don't credit one with the other's work.

**Done when:** you can hand it a bad line and it can tell you which principle the line breaks.

---

## 07 · Design System

**What it is:** the brand book, translated into rules an agent can execute. A brand PDF is for humans; this is the machine edition.

**What goes in it:**
- The palette as exact values, with the job each color does.
- Type, logo, and layout rules written as instructions, not examples.
- The creative modes: the few layouts the work is allowed to take.
- Hard rules stated as hard rules.
- Image-generation prompt templates that encode all of the above.

**The design decision:** uploading the brand-guide PDF makes the agent an archivist. Rewriting it as rules makes it a designer. That translation is where your judgment enters.

**Name the canonical source, out loud.** If more than one kit exists — a studio identity and an expanded one, a website theme and a brand guide — say which one governs and which one is off-limits, or the model picks by proximity. And note: *the artifact in production is not the source of truth.* A color sampled from the live site is not a brand color.

**Done when:** the agent can produce something on-brand without seeing an example.

---

## 08 · Brand Asset Index

**What it is:** every real file — logos, patterns, photos — mapped and described in plain words, so the agent picks assets by reading.

**What goes in it:**
- The folder map, exactly as the files live on disk.
- One line per file: what it shows, and what it's for.
- Retrieval rules: which folders each kind of task may pull from.
- Scope warnings: assets that exist but are off-limits for certain work.

**The design decision:** the agent does the looking, once. Point it at the folder and it writes a description of every file — that's the vision pass, and it's the cheap part. After that it works from text: picking the right asset without loading the image library every session, on any model, vision-capable or not.

**Done when:** the agent can build a full campaign without ever asking "which logo?"

---

## 09 · The Workflow

**What it is:** the operating loop, written down like any other context — including exactly where a human says yes.

**What goes in it:**
- The loop, step by step: ideate → draft variants → review → publish → measure → learn.
- The approval gates, named. Nothing spends, publishes, or changes without a human yes.
- What the agent may do freely: drafting, analysis, recommendations.
- Where learnings get saved, so the next cycle starts smarter.

**The design decision:** the process is context too, so it gets written down. When the brain moves to a more autonomous stack, the gates move with it. They live in the files, not in your head.

**Done when:** someone could hand the brain to a different operator and the gates would still hold.

---

## 10 · The Instructions Layer

**What it is:** the system prompt, kept deliberately lean. It does almost nothing but point.

**What goes in it:**
- The role, in two sentences: who the agent is, and what winning means.
- The hard rules, restated once: the ones that override everything.
- The routing map: which doc answers which kind of question.
- What to do when docs conflict, and when to say "unconfirmed."

**The design decision:** the mirror copy is the trick — keep a copy of this layer inside the knowledge base too. Then nothing load-bearing lives in a settings field, and the whole brain, operating rules included, moves to any stack as a folder of files.

**Done when:** you could paste it into a different tool tomorrow and lose nothing.

---

## 11 · The Decision Log — the doc that should exist

Here's the honest part.

The original build doesn't have this doc. It was reconstructed later, painfully, by reading the brain's own prohibition language and reverse-engineering what must have gone wrong to produce each rule. Every hard rule in a mature brain is a fossilized mistake — and six months on, nobody remembers which mistake.

**What goes in it,** one entry per rule that isn't obvious:
- **The rule.** As stated in whichever doc carries it.
- **What happened.** The mistake, the bad output, the near-miss, the thing that cost money.
- **What we rejected.** The other options considered, and why they lost.
- **What would reverse it.** The condition under which this rule stops applying.

**The design decision:** rules without reasons are cargo cult. A stranger inheriting your brain can follow the rules but can't know when they've expired — and neither can you, later, because you'll have forgotten.

Designed rules and scars read differently. Designed rules say *do this*. Scars say *never this*, and name the specific wrong thing. **When you catch yourself writing a "never," stop and log it.** That's the cheapest this will ever be.

**Done when:** every "never" in the brain has an entry.

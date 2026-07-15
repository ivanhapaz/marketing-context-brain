# Principles, and the scars behind them

The design decisions that make a context brain work, and the mistakes that produced them. Follow these while you build; teach the ones that apply.

Two kinds of rules live in a mature brain. **Designed rules** say *do this*. **Scars** say *never this*, and name a specific wrong thing. Scars are more valuable, because someone paid for them.

---

## The thirteen

**0. Never make them produce what you can go get. Always take what they already have.**
You're the specialist they hired, and they're probably a competent marketer with material in a folder. Ask for artifacts, not answers — *"do you have a competitor deck, or should I build one?"* Existing material beats your research on speed and tells you how they think. What doesn't exist, go get yourself when possible: market research, customer evidence, product or campaign analysis, the copy audit, the vision pass. Never send a client off to do homework you could have done.

**1. Spine first, thin — then re-audit it last.**
It's the router. It gets written by the least-informed version of the project and it ages worst. On the original build, the spine's document map still listed two of the biggest docs as "still to build" long after both existed. The staleness *was* the timestamp. Treat the map like code.

**2. Verify premises against live systems early, not last.**
*Scar.* On the original build, live systems were queried after nine docs existed — and immediately falsified a premise sitting in the spine, which had already propagated into three downstream docs. One wrong upstream assumption, four fixes. Pull the real data first. Let it correct the story before the story hardens.

**3. Two docs, two speeds.**
A depth doc and a quick reference. Agents, like people, reach for the quick one far more often, so make the quick one excellent.

**4. Anonymize at ingestion.**
Patterns in, identities never. You can't leak what you never loaded, and the analysis loses nothing.

**5. Translate the brand guide; don't attach it.**
Attaching a PDF makes the agent an archivist. Rewriting it as executable rules makes it a designer. The translation is where user judgment enters.

**6. Let the model look once, then work from text after.**
The vision pass is the agent's job: ask client to point you at the folder, you describe every file, the descriptions are banked. Vision costs tokens and latency; prose costs neither. One pass and the agent picks correctly forever — on any model, vision-capable or not.

**7. Make taste testable.**
A ✅ line and a ❌ line beat any adjective. The point isn't documentation, it's that the agent can check its own output before the client sees it.

**8. Restate the unbreakable rule everywhere. State everything else once.**
The original build repeats exactly one rule in all ten doc headers — the language rule that must never break. Redundancy is the feature: any doc might be the only one loaded. Everything else appears once, or it drifts.

**9. Put uncertainty on the output path.**
Research docs carry caveats sections. Output docs carry inline `(confirm)` flags. Mark uncertainty at the point where a claim is about to become an ad, not where it was born.

**10. Use proportional evidence standards.**
Do not turn assumptions into facts, but do not demand enterprise-grade attribution from a team that operates on founder calls, a small customer set, or incomplete systems. Mark what is verified, observed, chosen, or hypothesized. Narrow claims when necessary; leave a whole document unwritten only when there is no useful basis for it.

**11. Date every snapshot of a moving number — and write the re-audit instruction into the doc.**
Prices, packaging, market stats, benchmark claims, competitor claims, and other moving facts. The doc should say when it was true and when to check again.

**12. Stable section numbers are the addressing scheme.**
Cross-references are surgical (`Voice §2 P7`). Numbering looks cosmetic. Renumber and the graph breaks.

---

## The scars, and what caused them

These are real, reverse-engineered from the prohibition language in one working brain (a regulated-ads build). Yours will be different scars. The *shape* is the part that transfers: a rule that names a specific wrong thing is a rule someone paid for.

**"The website's theme color is not a brand color, and must never be used."**
Something sampled the live site and treated it as canonical.
→ *The artifact in production is not the source of truth.*

**"The second kit is website-only. Do not pull it for ads."**
Two identity kits existed. The wrong one was reachable.
→ *Name the canonical source out loud, or the model picks by proximity.*

**"Pronoun decision (resolved)."**
The word *resolved* is the scar. It marks a question that got asked twice.
→ *Some decisions reopen forever unless you record that they're closed.*

**"Never advertise a higher monthly figure. Never a price per unit."**
An early number got used, then a real dated quote contradicted it.
→ *Say which numbers are dead, not just which are alive.*

**A banned claim family, with ❌ example lines.**
An ad account died for this one.
→ *The rule that cost the most to learn gets the clearest examples.*

**A corrected industry claim.**
A confident, false, widely-repeated thing that everyone in the category says.
→ *Category common knowledge is often just category folklore. Check the claim everyone makes.*

**"Think in [working language]. Produce in [audience's native language], never translated."**
English-first drafting produces second-language copy that reads translated.
→ *If your audience isn't in your working language, separate the two layers explicitly — and put the rule in every doc.*

---

## What the docs can't hold

The docs record verdicts, not arguments. From the original build, none of this survived in writing:

- **The deliberation.** "Resolved" is a headstone. The debate is gone.
- **Rejected options.** Nothing records what was proposed and killed, or why.
- **The AI's errors.** A misread data pool, two numbers conflated into a false crisis, an entire platform audit sitting unnoticed in chat. None of it in any doc — and it's the most instructive material in the build.
- **Sequence and effort.** Multiple sessions over days. The docs present as though authored at once.
- **Dead ends.** A file too large to open. A login wall. Searches that returned nothing.
- **Stakes.** Why the project exists, who it's for, what it's really proving. Invisible, and it shaped every call.

This is the argument for doc 11. Every scar above had to be reverse-engineered from prohibition language, months later. It should have been written down when it was cheap.

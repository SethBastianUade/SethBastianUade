# Constitutional AI

<sub>Status: &nbsp;Reading · &nbsp;Updated: 2026-07-17</sub>

---

## Summary

A training approach where a model is improved by asking it to critique and revise its own outputs against a written constitution of principles, then supervised on the revisions. Reduces reliance on per-example human labelling.

## Current understanding

Constitutional AI exchanges "human rates every response" for "human writes the principles; model edits and grades against them." Useful at scale, but shifts the question to: where do principles come from, which contradictions matter, and how do we measure whether the model actually internalised them.

For engineers: it is a checkpoint in the training stack, not a substitute for evaluation. Constitutions drift silently unless audited.

## Resources

- [ ] *Constitutional AI: Harmlessness from AI Feedback* — Bai et al., Anthropic
- [ ] Anthropic follow-up on *Sleeper Agents* (limits of CAI-style training)
- [ ] OpenAI rule-based rewards work
- [ ] *The Calibration of Constitutional AI* — community analyses

## Notes

- _2026-07-17_ — Initial entry. Reading the original paper this week.

## TODO

- [ ] Re-read paper; write a structured summary focused on training data flow.
- [ ] Catalogue which principles measurably change behaviour vs. not.
- [ ] Survey known limitations: sleeper behaviour, principle conflicts, gaming.
- [ ] Prototype a small CAI-style revision loop on a local model.

## Open questions

- Who writes the constitution, and how is it amended safely?
- Can a constitution be *tested* instead of only stated?
- Does constitutional training compose with RLHF, or partially replace it?

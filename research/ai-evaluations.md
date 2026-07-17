# AI Evaluations

<sub>Status: &nbsp;Reading · &nbsp;Updated: 2026-07-17</sub>

---

## Summary

Procedures for measuring what a model can and cannot do — capability, safety, and behaviour. Evaluations are infrastructure: designed, versioned, reproducible, and run against specific model versions and system configurations.

## Current understanding

Three layers of evals:

- **Automatic** — cheap, high-signal only for narrow tasks.
- **Model-graded** — LLM-as-judge, scales but inherits model bias.
- **Human** — slow, expensive, ground truth.

Most production gaps come from conflating benchmark scores with deployment behaviour. Useful evals are tied to a threat model and a deployment context, not to a leaderboard.

## Resources

- [ ] *Evals Done Right* — OpenAI / contributions to the evals framework
- [ ] *Sleeper Agents: LLMs trained to be deceptive* — Hubinger et al.
- [ ] Anthropic safety-biology evaluations work
- [ ] Inspect AI framework (UK AISI)
- [ ] *Are Emergent Abilities a Mirage?* — Schaeffer et al.

## Notes

- _2026-07-17_ — Initial entry. Comparing Inspect AI with homegrown harnesses.

## TODO

- [ ] Set up a minimal eval harness in `experiments/llm-eval-001`.
- [ ] Define one capability eval and one safety eval from scratch.
- [ ] Document failure modes of LLM-as-judge observed in practice.
- [ ] Compare rubric grading vs. pairwise grading on the same dataset.

## Open questions

- How do we eval behaviours that only emerge at scale?
- What is the smallest eval set that meaningfully predicts deployment risk?
- How can evals resist Goodharting once they become targets?

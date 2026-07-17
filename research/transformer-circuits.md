# Transformer Circuits

<sub>Status: &nbsp;Reading · &nbsp;Updated: 2026-07-17</sub>

---

## Summary

Reverse-engineering the internal algorithms a transformer learns, expressed as circuits of attention heads and MLP sublayers. The original Anthropic interpretability thread.

## Current understanding

Transformers compose compositional circuits. Attention heads act as small primitives — copy, previous-token, induction — that combine into richer algorithms. Induction heads appear to be a key substrate of in-context learning.

This thread treats the model as an object we can read. It is the clearest existing bridge from low-level parameters to high-level behaviour, but currently only for small models and clean phenomena.

## Resources

- [ ] *A Mathematical Framework for Transformer Circuits* — Elhage et al.
- [ ] *In-context Learning and Induction Heads* — Olsson et al.
- [ ] *Toy Models of Superposition* — Elhage et al.
- [ ] *Smooth Elicitation* and follow-ups
- [ ] Anthropic Transformer Circuits thread (full archive)

## Notes

- _2026-07-17_ — Initial entry. Beginning with the framework paper.

## TODO

- [ ] Reproduce the induction-head detection metric on GPT-2 small.
- [ ] Reimplement the "previous-token head" finding.
- [ ] Write a summary aimed at backend engineers (analogy: traces vs. circuits).
- [ ] Catalogue which results have and have not survived to frontier models.

## Open questions

- Why are some circuits clean and others not?
- How does composition change under instruction tuning?
- Is there a circuit-level account of refusals and of "#1 assistant" behaviour?

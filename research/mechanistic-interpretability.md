# Mechanistic Interpretability

<sub>Status: &nbsp;Reading · &nbsp;Updated: 2026-07-17</sub>

---

## Summary

The study of which internal computations inside a neural network produce its behaviour. Goal: move from inspecting inputs/outputs to inspecting the learned circuits, with the aim of auditing, steering, and predicting models from the inside.

## Current understanding

Mostly empirical. Progress so far comes from small models (attention head circuits, induction heads), sparse-autoencoder feature discovery on larger models, and targeted probing. The field is far from a clean theory — most results are model-specific and fragile.

For engineers: interpretability is the bridge from "it works" to "I can give a justified reason it will keep working under distribution shift."

## Resources

- [ ] *Mathematical Framework for Transformer Circuits* — Elhage et al., Anthropic
- [ ] *In-context Learning and Induction Heads* — Olsson et al.
- [ ] *Language Models Can Explain Neurons in Language Models* — OpenAI
- [ ] *Scaling Monosemanticity* — Templeton et al., Anthropic
- [ ] Neel Nanda's interpretability course & ARENA material
- [ ] TransformerLens documentation

## Notes

- _2026-07-17_ — Initial entry. Starting with the Anthropic mathematical framework series.

## TODO

- [ ] Work through TransformerLens tutorial end-to-end.
- [ ] Reproduce induction-head detection on a small model.
- [ ] Write a short note translating a circuit result into engineering implications.
- [ ] Track limitations: polysemanticity, dataset dependence, training-time drift.

## Open questions

- Do circuits found in small models survive in frontier models?
- How much of interpretability transfers across model families?
- When is a "feature" real and when is it an artefact of the probe?

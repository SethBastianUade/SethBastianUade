# Agent Safety

<sub>Status: &nbsp;Reading · &nbsp;Updated: 2026-07-17</sub>

---

## Summary

Failure modes of autonomous systems built on LLMs — tool use, memory, planning loops, recursive calls — and the controls needed to keep their longhorizon behaviour inside intended bounds.

## Current understanding

An agent is not just a model; it is a control loop around a model. Most safety work in production is *scaffolding* — permission scopes, human-in-the-loop checkpoints, state sanitisation, capability allowlists, replanning limits.

Open problems compound at horizon: state drift, goal drift, compounding tool errors, and the fact that a strong model plus a fragile harness is often more dangerous than either alone.

## Resources

- [ ] Anthropic, Claude Code and agentic safety write-ups
- [ ] *Scheming Reasoning Evaluation* — Anthropic
- [ ] Apollo Research work on deception
- [ ] UK AISI agent evaluations
- [ ] OpenAI Preparedness Framework

## Notes

- _2026-07-17_ — Initial entry. Mapping agent failures to backend system failures.

## TODO

- [ ] Build a minimal agent harness with explicit permission surface.
- [ ] Catalogue failure categories: action, observability, side-effect, goal drift.
- [ ] Design a logging schema that makes post-hoc failure review tractable.
- [ ] Write a note on "least capability" as the agent analogue of least privilege.

## Open questions

- How should an agent escalate uncertainty?
- What is the unit test equivalent for an agentic loop?
- Can oversight models catch failures at the same horizon as the actor?

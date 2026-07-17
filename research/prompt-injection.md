# Prompt Injection

<sub>Status: &nbsp;Reading · &nbsp;Updated: 2026-07-17</sub>

---

## Summary

Indirect and direct manipulation of language model behaviour through crafted inputs embedded in prompts, retrieved context, or tools. First-order reliability problem for any system that lets an LLM touch untrusted data.

## Current understanding

LLMs follow instructions embedded in data they read, not just in the conversation they hold with the user. The boundary between *instruction* and *data* is not enforced by the model itself. Most mitigations today are system-level (privilege separation, allowlists, output filtering) rather than learned defences.

Deeper issues: indirect injection through retrieved documents, tool outputs, emails, and web pages is the realistic threat surface for agents.

## Resources

- [ ] *Not what you've signed up for: Defending Against Injection Through Indirect Prompt Instructions* — Greshake et al.
- [ ] OWASP LLM Top 10 — LLM01: Prompt Injection
- [ ] *Indirect Prompt Injection on GitHub Copilot Chat* — community reports
- [ ] Anthropic, Claude model card — security sections

## Notes

<!-- Append dated entries. Keep short. -->

- _2026-07-17_ — Initial entry. Started collecting incidents from real deployments.

## TODO

- [ ] Reproduce a minimal indirect-injection demo against a tool-using agent.
- [ ] Catalogue failure modes: data exfil, tool abuse, instruction override.
- [ ] Survey detection vs. prevention vs. isolation approaches.
- [ ] Write note comparing system-prompt defences vs. architectural isolation.

## Open questions

- Can instruction/data separation be enforced by training rather than scaffolding?
- Is "trust levels for context" a useful formalisation?
- How should an agent behave when two trusted sources give conflicting instructions?

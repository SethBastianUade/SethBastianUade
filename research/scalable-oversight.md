# Scalable Oversight

<sub>Status: &nbsp;Reading · &nbsp;Updated: 2026-07-17</sub>

---

## Summary

Methods that let a weaker overseer supervise a stronger actor well enough that supervision quality does not collapse as the actor's capability grows past the overseer's. Crucial if we expect to train future models from weaker human or model graders.

## Current understanding

Core tension: as the supervised system gets smarter, the supervisor loses ground. Proposals — debate, recursive reward modelling, AI safety via debate, weak-to-strong generalisation — try to keep supervision effective even when the supervisor cannot fully audit the work.

No proposal currently solves the " Walt Disney / lazy oversight" case where the actor produces output the supervisor cannot meaningfully verify.

## Resources

- [ ] *AI Safety via Debate* — Irving et al.
- [ ] *Scalable Ovesight via Weak-to-Strong Generalisation* — Burns et al., OpenAI
- [ ] *CriticGPT* and follow-up work — OpenAI
- [ ] Anthropic, *Recursive Reward Modelling*
- [ ] *Weak-to-strong generalisation* — recent follow-ups

## Notes

- _2026-07-17_ — Initial entry. Drawing parallels to code review at scale.

## TODO

- [ ] Reproduce a weak-to-strong experiment on a small task.
- [ ] Compare single-grader vs. debate vs. ensemble grading settings.
- [ ] Write a note mapping alright oversight onto backend code review practice.
- [ ] Track where oversight fails as model capability rises.

## Open questions

- Is supervision bounded by the supervisor, or can it be lifted by structure?
- When does monitoring beat grading?
- How does oversight survive hidden context (state an overseer cannot see)?

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/hero-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/hero-light.svg">
    <img alt="Sebastián Arroyo — Building Reliable Software. Studying Reliable AI." src="./assets/hero-light.svg" width="100%">
  </picture>
</div>

<br/>

<div align="center">
  <a href="https://sebastianarroyo.tech">Portfolio</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/SethBastianUade">GitHub</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://www.linkedin.com/in/sebasti%C3%A1n-arroyo-84a46a20a/">LinkedIn</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="mailto:sebastianarroyo9014@gmail.com">Email</a>
</div>

---

## Mission

This repository is a public log of my transition from backend engineering into AI safety and AI engineering.

I spend my days building reliable software — Java, Spring Boot, well-shaped APIs — and my evenings studying what it would take to build **reliable AI**. I document the work in the open: notes, reading, small experiments, and the things I get wrong along the way.

The intended output is not a portfolio. It is a long-running notebook, kept for years, that records how an engineer actually moves into this field — one paper, one eval, one failed reproduction at a time.

---

## Research Timeline

A working history. Intentionally incomplete — milestones get added as they happen.

<pre>
2024 ──┐
       │  Started Software Engineering
       │
2025 ──┤
       │  Professional Java Backend Engineer
       │
2026 ──┤
       │  Selected for BlueDot Technical AI Safety
       │
Now  ──┤
       │  Building Kreta
       │
Now  ──┤
       │  Learning AI Safety · Alignment · LLM Reliability
       │
Next ──┤
       │  AI Alignment Engineering
       │
...   └─ future entries
</pre>

---

## Research Log

A live laboratory notebook. Each topic is a working file under [`/research`](./research). Most entries are preliminary — they grow as understanding does.

&nbsp;&nbsp;<sub>Status legend: &nbsp;`Reading` active study · `Drafting` summary stable · `Working` running experiments · `Revisited` returned to after a gap</sub>

| Status | Topic | Summary | Notes |
| :---: | --- | --- | :--- |
| Reading | [Prompt Injection](./research/prompt-injection.md) | Instruction/data boundary inside LLM systems | placeholders |
| Reading | [Mechanistic Interpretability](./research/mechanistic-interpretability.md) | Reverse-engineering internal model computation | placeholders |
| Reading | [AI Evaluations](./research/ai-evaluations.md) | Capability and safety evals as infrastructure | placeholders |
| Reading | [Transformer Circuits](./research/transformer-circuits.md) | Attention and MLP circuits, induction heads | placeholders |
| Reading | [Agent Safety](./research/agent-safety.md) | Failure modes of autonomous LLM loops | placeholders |
| Reading | [Scalable Oversight](./research/scalable-oversight.md) | Supervising stronger actors from weaker ones | placeholders |
| Reading | [Constitutional AI](./research/constitutional-ai.md) | Self-critique against written principles | placeholders |

> Topics are added as I start them. Files I have not yet opened are not listed here.

---

## Current Reading

A queue, tracked honestly. Bars show where I am; links go to notes when they exist.

<table>
  <tr><td>

**AI Safety Fundamentals** &nbsp;— *BlueDot curriculum*
`██████████░░░░░░░░░░` &nbsp; 50% &nbsp;·&nbsp; <sub>Reading</sub> &nbsp;·&nbsp; <sub><i>notes pending</i></sub>

**Mathematical Framework for Transformer Circuits** &nbsp;— *Elhage et al.*
`████░░░░░░░░░░░░░░░░` &nbsp; 20% &nbsp;·&nbsp; <sub>Reading</sub> &nbsp;·&nbsp; <sub><i>notes pending</i></sub>

**In-context Learning and Induction Heads** &nbsp;— *Olsson et al.*
`██░░░░░░░░░░░░░░░░░░` &nbsp; 10% &nbsp;·&nbsp; <sub>Queued</sub>

**Language Models Can Explain Neurons in Language Models** &nbsp;— *OpenAI*
`░░░░░░░░░░░░░░░░░░░░` &nbsp;&nbsp;0% &nbsp;·&nbsp; <sub>Queued</sub>

**Constitutional AI** &nbsp;— *Bai et al., Anthropic*
`██░░░░░░░░░░░░░░░░░░` &nbsp; 10% &nbsp;·&nbsp; <sub>Queued</sub>

</td></tr>
</table>

<details>
<summary><sub> backlog — papers queued for later (click to expand) </sub></summary>

- [ ] &nbsp;*Toy Models of Superposition* — Elhage et al.
- [ ] &nbsp;*Sleeper Agents* — Hubinger et al.
- [ ] &nbsp;*Scaling Monosemanticity* — Templeton et al.
- [ ] &nbsp;*AI Safety via Debate* — Irving et al.
- [ ] &nbsp;*Are Emergent Abilities a Mirage?* — Schaeffer et al.
- [ ] &nbsp;*Not what you've signed up for* — Greshake et al.
- [ ] &nbsp;<sub>placeholder — add next paper</sub>

</details>

---

## Experiments

Small implementations to test understanding. Most fail or produce noise. That is the point.

| Status | Name | What it tests | Repo |
| :---: | --- | --- | --- |
| Planning | `llm-eval-001` | A minimal capability + safety eval harness from scratch | _coming_ |
| Planning | `induction-heads` | Reproduce induction-head detection on GPT-2 small | _coming_ |
| Planning | `inject-lab` | A controlled indirect-prompt-injection testbed against a tool-using agent | _coming_ |
| Planning | `weak-to-strong` | Minimal weak-to-strong generalisation experiment | _coming_ |
| Planning | `agent-harness` | An LLM agent with an explicit, auditable permission surface | _coming_ |

> Empty repos are not created until I have time to start them. Names are reserved.

---

## Lab Notes

Short, dated entries. Easy to maintain by hand. Newest on top.

&nbsp;&nbsp;**2026-07-17** &nbsp;— Started this notebook publicly.
&nbsp;&nbsp;Kreta continues in parallel; research log begins here.

&nbsp;&nbsp;**2026-07-15** &nbsp;— Accepted into BlueDot Technical AI Safety.

&nbsp;&nbsp;**2026-07-** &nbsp;— _placeholder_

<!--
Append new entries as:
&nbsp;&nbsp;YYYY-MM-DD — one-line note.
Keep the most recent at the top of the dated list.
-->

---

## Open Questions

Things I cannot answer yet and am actively thinking about. Listed to show what I am working toward, not what I claim.

- How should we evaluate reasoning rather than retrieval?
- What practical interpretability techniques transfer from small to frontier models?
- How can agent failures — long-horizon, sparse, compounding — be measured before deployment?
- Is instruction/data separation a property we can train, or only scaffold?
- What is the smallest meaningful eval set that predicts deployment risk?
- Can oversight keep up when the actor outpaces the overseer?
- How do we detect when a model has internalised a principle versus learning to recite it?

> Added as I notice them. Never removed; downgraded to a Research Log entry when answered.

---

## Focus Areas

<table>
  <tr>
    <td width="50%" valign="top">
      <strong>Engineering</strong><br/>
      <sub>Java · Spring Boot · System Design · Enterprise APIs</sub>
      <br/><br/>
      ·&nbsp; Backend services with clear architecture<br/>
      ·&nbsp; Maintainable, observable systems<br/>
      ·&nbsp; Developer tooling and DX
    </td>
    <td width="50%" valign="top">
      <strong>Research</strong><br/>
      <sub>AI Safety · Alignment · LLM Reliability</sub>
      <br/><br/>
      ·&nbsp; Reliable AI systems<br/>
      ·&nbsp; Model evaluations<br/>
      ·&nbsp; Mechanistic interpretability
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong>Building</strong><br/>
      <sub><a href="https://github.com/SethBastianUade">Kreta</a> — home for modern software and AI products</sub>
      <br/><br/>
      Early-stage work where backend reliability meets applied AI.
    </td>
    <td width="50%" valign="top">
      <strong>Learning</strong><br/>
      <sub>BlueDot — Technical AI Safety</sub>
      <br/><br/>
      Structured study of fundamentals, alignment, and frontier risks.
    </td>
  </tr>
</table>

---

## Stack

<div align="center">

<img src="https://img.shields.io/badge/Java-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="Java"/>
&nbsp;<img src="https://img.shields.io/badge/Spring%20Boot-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="Spring Boot"/>
&nbsp;<img src="https://img.shields.io/badge/Python-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="Python"/>
&nbsp;<img src="https://img.shields.io/badge/Docker-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="Docker"/>
&nbsp;<img src="https://img.shields.io/badge/PostgreSQL-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="PostgreSQL"/>
&nbsp;<img src="https://img.shields.io/badge/GitHub%20Actions-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="GitHub Actions"/>
&nbsp;<img src="https://img.shields.io/badge/React-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="React"/>
&nbsp;<img src="https://img.shields.io/badge/TypeScript-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="TypeScript"/>
&nbsp;<img src="https://img.shields.io/badge/OpenAI%20API-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="OpenAI API"/>
&nbsp;<img src="https://img.shields.io/badge/Claude%20Code-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="Claude Code"/>
&nbsp;<img src="https://img.shields.io/badge/Inspect%20AI-0B0F17?style=flat&labelColor=111827&color=94A3B8" alt="Inspect AI"/>

</div>

---

<div align="center">
  <sub>A notebook kept openly. Continuous learning, not finished work.</sub>
</div>

<br/>

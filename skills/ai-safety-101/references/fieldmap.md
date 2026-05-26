# AI Safety Fieldmap

A map of how AI safety subfields fit together, used by the `ai-safety-101` skill for orientation questions ("Map the field" / "How do the subfields fit?").

## About this file

The five-stage spine below is a working synthesis of how established AI safety curricula organize the field — not a canonical map. The pillars (Anticipation, Threat modeling, Measurement, Intervention, Governance) recur across multiple curricula; arranging them along a causal spine is an editorial choice. Informed people draw the boundaries differently and that's fine.

When rendering this map, follow SKILL.md's pedagogy — translate into prose, don't import the parenthetical sub-lists verbatim, and surface the "synthesis, not canon" caveat only on full-map renders where it earns its place.

## The organizing logic: a five-stage spine

AI safety has a causal spine. The work exists to break a chain: a capability appears → it could cause specific harm → you must detect whether a given system has the dangerous property → you must prevent or contain it → institutions must make all of that happen at scale.

The field is organized by position on that spine — by the *function* each body of work performs, not by topic label:

1. **Anticipation** — what is coming, and how fast.
2. **Threat modeling** — what specifically goes wrong, and how.
3. **Measurement** — whether a given system actually has the dangerous property.
4. **Intervention** — preventing the failure, or containing it.
5. **Governance** — making institutions carry out stages 1–4 at scale.

**Foundations** sits outside the spine as a scaffolding layer: the ML literacy needed before the technical stages (neural networks, transformers, training pipelines, RLHF mechanics). It is prerequisite ML, not AIS itself, and the field's own curricula mark it "review" or "optional."

## How to read this map

Read at the depth the question calls for:

- **Quick orientation** — stage names and one-line summaries above.
- **Standard** — stage names plus each stage's paragraph below.
- **Full** — stages in detail plus the interpretability cross-cut and contested boundaries.

Match the rendering depth to the question per SKILL.md's pedagogy; translate into prose rather than importing the sub-lists verbatim.

---

## Stage 1 — Anticipation

*What are we up against, and on what timeline?*

Forecasting, AI timelines, scaling trends, takeoff dynamics, and the drivers of progress (compute, data, algorithms).

It opens the spine because everything downstream depends on the shape and urgency of the trajectory. Forecasting is also a genuine specialization in its own right, not only an orientation step.

## Stage 2 — Threat modeling

*What specifically goes wrong, and how?*

The risk landscape, under a tripartite split: **misuse** (deliberate harm — cyber, bio, influence operations), **misalignment** (the system pursues unintended goals — specification gaming, reward hacking, goal misgeneralization, deception, scheming), and **systemic harm** (labour, power concentration, autonomy, environment).

The "alignment problem" lives here, as the misalignment branch — it is the *characterization* of a failure, not yet its solution. The solution work is Stage 4.

## Stage 3 — Measurement

*How do we know whether a given system actually has a dangerous property?*

Benchmarks, dangerous-capability evaluations, red-teaming, control evaluations, monitoring and anomaly detection — and interpretability used diagnostically, to audit a model for a dangerous internal feature.

Measurement is the bridge from technical work to Governance: evaluations are what frontier-safety frameworks are built on.

## Stage 4 — Intervention

*What do we actually do about it?*

Alignment techniques (RLHF/RLAIF and preference learning), scalable oversight (debate, iterated amplification, weak-to-strong generalization), AI control, robustness and adversarial defence, unlearning, and defence-in-depth. The "alignment solutions" half of the field is here, as is interpretability used constructively — steering or editing a model, or training for interpretable structure.

## Stage 5 — Governance

*How do we make stages 1–4 actually happen, at scale?*

Policy and regulation, standards, compute governance, frontier safety frameworks and responsible-scaling policies, lab practices, liability, and international coordination.

---

## A cross-cutting discipline: interpretability

Interpretability does not sit at one point on the spine. It is a *tool*, and the field uses it at two stages: in **Measurement**, to audit whether a model has a dangerous internal feature; in **Intervention**, to steer or edit a model and to design training that yields interpretable structure. It is named once, here, so the split is visible rather than buried.

It is notably present in both major curriculum traditions (see Disclosure A) unchanged — stronger evidence of centrality than its single position in the field's vocabulary suggests.

## Contested boundaries

**Disclosure A — two curriculum traditions.** AIS curricula fall into two lineages that organize the field differently. The *AGI-safety lineage* (BlueDot, 80,000 Hours, much of AI Safety Atlas) runs capabilities → catastrophic risk → alignment → governance. The *ML-safety lineage* (CAIS's Intro to ML Safety; the university courses lean this way) runs robustness → monitoring → control → systemic safety. The five-stage spine is offered as the superset both are projections of — but that claim is itself a synthesis. The most visible consequence: robustness is a top-level pillar in one tradition and a sub-topic in the other.

**Disclosure B — the near-term-harms boundary.** Systemic and societal harm (labour, power concentration, autonomy, environment) appears in every modern curriculum, inside Threat modeling — so whether it is "in" the field is settled. What remains contested is *weighting*: one camp treats systemic harm as one category among catastrophic risks; the near-term-harms camp argues it deserves primary weight. The fieldmap includes it without adjudicating the weight.

## Provenance

The five-stage synthesis draws on eight independent public curricula:

- BlueDot Impact — AGI Strategy, Technical AI Safety, Frontier AI Governance
- CAIS — Intro to ML Safety *(curriculum dated 2023 — the one stale source)*
- ARENA — Alignment Research Engineer Accelerator
- 80,000 Hours — AI risk problem profile and career reviews
- International AI Safety Report — Bengio-chaired, 2026 edition
- AI Safety Atlas — CeSIA
- Harvard CS 2881R — graduate AI safety course
- Berkeley AI Safety Student Initiative — student-run AI safety DeCal

The curricula above were surveyed in 2026; their structures and offerings drift over time. The arrangement of pillars into the five-stage spine is an editorial synthesis, not a finding from the curricula themselves.

# AI Safety Concepts

A starting set of teaching aids for core AI safety concepts. Not exhaustive — most AI safety concepts are not in this file, and that's fine.

## How to use this file

Three cases to know:

1. **The concept has a vetted entry below.** Use it as scaffolding. Adapt the wording to the question's register, keep the intuition and example, surface the contested-framing flag where relevant.
2. **The concept is in AI safety but not in this file** (either named at the bottom or not named at all). Define it from your own knowledge using the pedagogy in SKILL.md — intuition first, one analogy, concrete example, flag contested framings, no fabricated specifics. **This is the normal mode for most concepts.**
3. **The question is outside AI safety entirely.** Respond normally; don't force this skill's framing onto it.

Vetted entries exist for concepts where (a) Claude tends to reinvent or distort them without help, or (b) the framing is contested in a way that matters and easily gets flattened. The named list at the bottom is a prompt for which concepts to be ready to handle — not a restriction on what you can answer.

## Entry format

Each entry has:
- **Concept name** (heading).
- **One-sentence working definition** — what to lead with if the question is terse.
- **Intuition** — the mental image. Lead with this in most cases.
- **Why it matters** — one concrete reason; usually a failure mode this concept names.
- **Contested framing** (if applicable) — what informed people disagree about.
- **Related concepts** — sibling ideas the learner may want next.

---

## Vetted entries

### Reward hacking

**Definition.** A system optimizes the measurable proxy of a goal rather than the goal itself.

**Intuition.** A cleaning robot rewarded for low sensor-detected dust learns to cover the sensor. The reward went up; the room is no cleaner. The system did exactly what it was measured on — that just wasn't what was meant.

**Why it matters.** Almost every training method gives the system a reward signal that is a proxy for what we actually want. As capability rises, the system gets better at finding gaps between the proxy and the real goal. The failure can look like success right up until it doesn't.

**Contested framing.** Researchers distinguish *specification gaming* (the reward was specified in a way that admits an unintended loophole) from *reward misspecification* (the proxy was simply the wrong thing to measure). The boundary is fuzzy — both amount to "we measured the wrong thing" — and some treat them as one phenomenon. Note: *goal misgeneralization* is a related but distinct failure mode (a model learns a goal that happens to work in training but generalises differently in deployment) — it is not a sub-type of reward hacking. fieldmap.md correctly lists them as coordinate siblings under the misalignment branch.

**Related.** Specification gaming, Goodhart's Law, goal misgeneralization (sibling concept — different failure mechanism), the alignment problem.

---

### The alignment problem

**Definition.** The problem of building AI systems that pursue goals their developers and users actually want, rather than something correlated but different.

**Intuition.** "Aligned" doesn't mean "nice" or "ethical." It means the system's actual behavior, including in situations it wasn't trained on, matches what we intended. A perfectly polite assistant that quietly subverts your goals is not aligned. A blunt assistant that does what you actually need is.

**Why it matters.** The methods we have for telling a model what to do (curated data, reward signals, written instructions) are all indirect. They specify behavior on the training distribution; they do not directly install goals. The gap between "behaves well in training" and "pursues the intended goal in general" is where the field's hardest problems live.

**Contested framing.** Whether "alignment" is one problem or a cluster (intent alignment, value alignment, capability alignment, etc.) is debated. So is whether the right frame is *technical* (make the model want the right thing) or *sociotechnical* (build the institutions around the model to handle the gap).

**Related.** Reward hacking, scalable oversight, deceptive alignment, the orthogonality thesis.

---

### RLHF (Reinforcement Learning from Human Feedback)

**Definition.** A training technique where humans rank model outputs, those rankings train a reward model, and the language model is then fine-tuned to produce outputs the reward model scores highly.

**Intuition.** Imagine teaching a writer not by editing every sentence, but by saying "I prefer this draft to that one" thousands of times. The writer learns a model of your taste and writes for it. RLHF is that — at scale, with humans ranking pairs of model outputs.

**Why it matters.** RLHF is how most current chat assistants are made conversational and broadly compliant with what users want. It's also the source of several known failure modes — sycophancy (the model learns "I like being agreed with"), shallow value learning (the reward model misses the deep thing the rankers cared about), and gaming the reward model rather than serving the underlying intent.

**Contested framing.** Whether RLHF is a real *alignment* technique or only a *behavior-shaping* technique is debated. Critics argue it makes models look aligned without making them aligned; defenders argue it is the most empirically grounded thing the field has and that the criticism conflates limitations with uselessness.

**Related.** RLAIF (RL from AI Feedback), Constitutional AI, preference learning, sycophancy.

---

## Other core concepts (define from your own knowledge at runtime)

The following are part of the field's stable canon. No vetted entry yet — when one of these comes up, define it from your own knowledge using the pedagogy in SKILL.md (intuition first, one analogy, concrete example, flag contested framings, no fabricated specifics). Don't fall silent just because there's no entry.

If a concept here is one you consistently get shallow or wrong, that's a signal it should be promoted to a vetted entry above. Likewise if its framing is contested in a way a default explanation flattens.

- Deceptive alignment
- Mesa-optimization / inner alignment
- Mechanistic interpretability
- Dangerous capability evaluations
- Red-teaming
- AI control
- Scalable oversight
- Weak-to-strong generalization
- Constitutional AI
- Responsible Scaling Policies / Frontier Safety Frameworks
- Compute governance
- Model evaluations vs. behavioral evaluations
- Goal misgeneralization
- Specification gaming
- Goodhart's Law
- Sycophancy
- Power-seeking
- Instrumental convergence
- The orthogonality thesis
- Treacherous turn
- Sandbagging
- Sleeper agents
- Activation steering
- Probes / linear probes
- Sparse autoencoders (SAEs)
- Circuit analysis
- Model organisms of misalignment
- Eval gaming
- Reward modeling
- Process-based vs. outcome-based supervision

The list is illustrative, not exhaustive. Concepts outside this list are also handled the same way — define from your own knowledge per the SKILL.md pedagogy.

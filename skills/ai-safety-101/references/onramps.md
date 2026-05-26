# AI Safety Onramps

Curated entry points to the field for newcomers: curricula, reading lists, intro courses, and primary writers. Used by the `ai-safety-101` skill for "where do I start" and "what should I read" questions.

## About this file

This file contains some recommended starting points for AI safety beginners — curricula, reports, and intro articles. The list is not exhaustive and can be updated over time.

URLs and program details may drift. With web search available, verify a link still resolves and the program is still active before sharing it; use the updated URL if it has changed. Without web search, use entries as written and surface the entry's `last_verified` date so the user can check directly.

For details not in the file (current cohort dates, application deadlines, pricing): say plainly you don't have those. With web search you may look them up and cite the live source separately; without it, point the user to the program's site.

## How to use this file

- Trigger on questions like "where do I start", "what should I read", "what are good intro resources", "how do I learn AI safety".
- Match the recommendation to the person's background:
  - **No technical background** → narrative/conceptual entries first (80,000 Hours problem profile, AI Safety Atlas chapters 1–2, books).
  - **Technical / ML background** → curricula with hands-on components (ARENA, BlueDot Technical, CAIS).
  - **Policy/governance background** → BlueDot Frontier AI Governance, GovAI primers, International AI Safety Report.
  - **Cross-disciplinary (PM, design, ops)** → AI Safety Atlas + governance reading + one applied project.
- For **upskilling questions** (structured learning sequences, program comparisons like BlueDot vs ARENA vs AISES, "what should I learn to do X," "walk me through a path to become competent in Y"), route to `ai-safety-learning-paths` *if it is loaded*. If it is not loaded, handle the question here: use this file's first-reading entries plus sensible sequencing, and give a complete self-contained answer. Do not tell the user about the existence of any other skill — that framing leaks implementation details they have no visibility into.
- Do not recommend more than 3–4 resources per response. A long list paralyses; a short one gets opened.

## Entry format

Each entry has:
- **Name** (heading).
- **Type** — curriculum / book / paper / report / blog.
- **Best for** — one line on the audience.
- **Time investment** — rough estimate.
- **Notes** — strengths, caveats, prerequisites.
- **URL** — primary link.
- **`last_verified`** — date the entry was last checked.

---

## Entries

### Foundational curricula

- **BlueDot Impact courses** — AGI Strategy, Technical AI Safety, Frontier AI Governance, plus an AI Safety Operations Bootcamp and a Technical AI Safety Project Sprint for graduates. Type: structured curriculum (cohort or self-paced). Best for: people who want a guided sequence with peers; main entry point into the field for many. Time: ~6–10 weeks part-time per course. URL: https://bluedot.org/courses. *`last_verified`: 2026-05-25.*

- **AI Safety Atlas (CeSIA)** — open textbook by Markov Grey, Charbel-Raphaël Segerie et al. Best for: cross-disciplinary self-study; chapter 1 in particular for newcomers. Comprehensive coverage from capabilities and risks through interpretability and oversight. Time: read selectively. URL: https://ai-safety-atlas.com. *`last_verified`: 2026-05-25.*

- **ARENA (Alignment Research Engineer Accelerator)** — Best for: people with ML/coding background who want hands-on technical experience. Format: 4–5 week in-person bootcamp at LISA, London (currently ARENA 8.0); curriculum also available self-paced online. Covers transformer interpretability, RL, LLM evals, model organisms of misalignment. URL: https://www.arena.education (program) / https://learn.arena.education (self-paced curriculum). *`last_verified`: 2026-05-25.*

- **CAIS Intro to ML Safety** — Best for: ML-literate learners on the technical/empirical-safety side of the field. Created by Dan Hendrycks; covers robustness, monitoring, control, systemic safety. Time: self-paced (~8 weeks at 5 hrs/week). Notes: most recent run was Spring 2023; underlying material reflects that vintage but still useful as a structured empirical-safety primer. URL: https://course.mlsafety.org. *`last_verified`: 2026-05-25.*

### Reports and overviews

- **International AI Safety Report** (Bengio-chaired). Type: synthesis report; second edition published February 2026, authored by 100+ international experts, backed by 30+ countries. Best for: an authoritative, recent state-of-the-field overview. Time: ~3–5 hours skim of the full report; ~20-page Extended Summary for Policymakers available separately. URL: https://internationalaisafetyreport.org. *`last_verified`: 2026-05-25.*

- **80,000 Hours AI risk problem profile** — now titled "Risks from power-seeking AI systems" (replaces the 2022 existential-risks profile; same lineage). Type: long-form web article. Best for: motivational/strategic framing of the case for AI safety, drawing on recent empirical evidence and addressing objections; especially good for career-curious readers. Time: ~1 hour. URL: https://80000hours.org/problem-profiles/risks-from-power-seeking-ai/. *`last_verified`: 2026-05-25.*

### Books and longer reads

Books age fast and recommendations depend on the user's background — not statically curated here. With web search available, look up current high-signal recommendations (canonical AI safety reading lists live at 80,000 Hours, AI Safety Atlas, and BlueDot). Without web search, point the user to those reading-list sources rather than recommending books from memory.

### Blogs and primary writers

Blog quality is high-variance — recommend specific posts, not whole blogs. With web search available, surface current high-signal posts on the user's topic. Common discovery surfaces: Alignment Forum, lab safety teams (Anthropic, OpenAI safety, DeepMind), evaluation organizations (Apollo Research, METR). Without web search, point to these surfaces rather than endorsing posts you can't verify.

---

## Notes for the model using this file

- **Don't invent programs not in this file.** The file's curation is what makes the recommendation trustworthy. With web search, you may verify a program a user asks about and cite the live source separately; without web, stick to what's listed and tell the user you don't have details on programs outside the file.
- **Match the audience.** A senior policy person doesn't need ARENA; a self-taught coder doesn't need Frontier AI Governance first. Ask one clarifying question if the question gives you nothing to infer from.
- **Hand off the upskilling version when possible.** If they ask "should I do BlueDot or ARENA to build my technical alignment skills?" route to `ai-safety-learning-paths` if loaded. If not, offer a reasonable comparison from what you actually know about the programs' focus, time commitment, and audience. Answer the question completely; do not refer to other skills.

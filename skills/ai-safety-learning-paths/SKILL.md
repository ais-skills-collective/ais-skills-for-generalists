---
name: ai-safety-learning-paths
description: >
  Build a personalised AI safety learning plan for people transitioning into the field.
  Use this skill whenever someone asks how to get into AI safety, what they should study,
  which fellowships or programs suit their background, how to upskill for an AIS role, or
  how to compare programs like BlueDot, AISES, ARENA, MATS, GovAI, or AGI Safety
  Fundamentals. Trigger even for vague intent like "I'm interested in AI safety, where do
  I start?" or "is my background relevant to AI safety?" Covers all career tracks:
  technical research, governance, communications, journalism, field-building, operations,
  evaluations/red-teaming, AI security, legal/regulatory, biosecurity, and policy.
---

# AI Safety Learning Paths

Help generalists and career-changers with AI safety learning queries. Answer their
specific question first using live sources, then offer to build a full personalised
learning plan only if they want one.

---

## How to engage the user

Memory comes first. Before asking the user anything, check what's already in your
context about them — Claude's memory of previous conversations, any user profile
information, anything they've shared earlier in the current conversation. If memory
gives you enough to be specific (their background, what they're working on, target
direction, relevant constraints), use it directly. Reference what you know naturally,
the way you would in any other conversation; don't make a show of recalling it. Don't
ask the user to re-share what you already know.

Once you've registered what memory gives you, decide which mode to operate in:

**Mode A — sufficient context (from memory, shared bio, or the query itself).** Give a
substantive, tailored answer immediately. If one specific piece would sharpen it further
(e.g. you know their background but not their geographic constraints, or you know their
target direction but not their seniority), ask one focused follow-up while answering —
don't withhold the answer waiting for it.

**Mode B — insufficient context.** Give a useful general answer to the asked question in
2-3 sentences so they aren't form-walled (this is the same step as "Answer the query
directly" in the Default Behaviour section below — not two separate responses). Then
invite them to share more for a tailored answer, naming three ways:

1. A paragraph in their own words covering what they've done, what they're aiming at,
   and any constraints
2. Their CV or LinkedIn pasted or uploaded (mention that for privacy they may want to
   redact identifying details — CV/bio is particularly useful because it captures career
   history and shipped work that memory may not have)
3. Answering a short set of questions if they prefer structured

Make the invitation feel like an offer, not a gate. If they decline or just want the
general answer, give them a good one and don't push.

The minimum useful information set — what to use from memory or ask for, depending on
what's missing:

- **Background**: current role, sector, rough years of experience
- **Target direction**: which AI safety area pulls them, or "I don't know yet" (a
  legitimate answer that changes how you respond)
- **Constraints that matter**: geography, full-time vs part-time, willingness to
  retrain, technical interest, financial runway
- **Existing engagement**: any AI safety work they've already done — reading, courses,
  projects, applications, public writing. This matters because it changes which pathways
  are realistic.

Tone: warm and conversational, not sycophantic. Treat the user as a peer who is new to
the field but not new to careers. Don't add congratulatory phrasing for "taking the
leap" or sharing their CV. Be direct and substantive. Plain language. No emojis unless
they use them.

---

## Default behaviour — answer first, plan second

When a user asks a question (e.g. "what should someone with a biotech background read?",
"is AI safety policy a viable career?"), do this:

1. **Answer the query directly** using web_search to fetch current information from the
   primary sources listed in Step 2. Give a focused, useful answer.
2. **At the end**, offer the learning plan: "Would you like me to build you a personalised
   learning plan based on your background and goals?"
3. **Only proceed to Steps 1–4 if they say yes** (or if they explicitly asked for a plan
   in their opening message).

**Program comparison queries** ("what's the difference between BlueDot and ARENA?",
"MATS vs LASR", "compare X and Y") skip Steps 1–4 entirely and go
directly to the **Handling Comparison Queries** section below. Queries like "which
fellowship should I apply to?" are recommendation requests, not comparisons — route
those through the intake flow (Steps 1–4) so you have the profile needed to advise.

This keeps the skill useful for one-off queries without forcing every user through a
full intake flow.

---

## Step 1 — Build the User Profile Progressively

Extract answers from the opening message first — never ask for something the user
already told you. Then follow the three-tier intake below. Move to the next tier only
when the current tier is answered.

### Tier 1 — Always ask (load-bearing, unlocks the plan)

Ask all three in a single opening message if not already known:

1. **Current background** — what field or role they're coming from
2. **Target role / track** — what kind of AIS work they want to do. "I don't know yet"
   is a completely legitimate answer here. If they're unsure, don't treat it as a
   blocker — use it as an opportunity to briefly orient them: explain that AI safety has
   several distinct entry paths (technical research, governance, communications, ops,
   evals, etc.), that most people start with a foundational course regardless of track,
   and that clarifying their direction is itself a useful early step. You can share the
   track list from Step 3 to help them locate themselves, but keep it light — the goal
   is orientation, not an exhaustive taxonomy.
3. **Time commitment** — full-time or part-time, and how many hours per week they can dedicate

These three together unlock a minimum viable plan. Never skip field 3 — it determines
which entire categories of programs are eligible. If field 2 is genuinely unknown, you
can still build a partial plan: recommend a foundational course that works across tracks
(e.g. BlueDot) and frame it as "step one regardless of where you end up."

### Full-time vs part-time filtering rule

Apply this filter before any recommendation:

- **Part-time (under ~20 hrs/week or still employed)**: recommend only self-paced
  courses, async cohorts, and online programs. Do not recommend residential fellowships,
  full-time bootcamps, or programs that require leaving employment. If a fellowship would
  otherwise be a strong fit, note it as a future option once their situation changes.
- **Full-time (20+ hrs/week or between roles)**: the full range of programs is eligible,
  including residential fellowships, intensive cohorts, and structured programs. However,
  do not recommend specific fellowships until background and track are also known — a
  full-time window doesn't tell you which fellowship fits. Ask for those first.

Always name the assumption: "Since you're part-time, I've focused on async options — if
your situation changes, [X fellowship] would be worth revisiting."

### Tier 2 — Ask if ambiguous after Tier 1

Ask only the fields that genuinely change the recommendation:

4. **Employment status** — employed / student / between roles; confirms feasibility of
   full-time programs (use this to cross-check field 3 if the two seem inconsistent)

If the user seems in a hurry, skip Tier 2 and note the assumptions you've made.

### Tier 3 — Ask only if highly relevant

Surface these only when the plan hinges on them:

5. **Location / timezone** — only ask if a fellowship you're about to recommend is
   in-person or heavily timezone-dependent
6. **Timeline** — only ask if the user hasn't implied urgency and the answer would change
   whether you sequence fast-track vs. long-term options
7. **Prior AIS exposure** — only ask if you'd recommend a beginner resource that would be
   redundant if they've already done it

---

## Step 2 — Fetch Current Resources

### Check web search availability first

Before searching, check whether web_search is enabled. If it is not available, tell the
user: "I'm working from a reference list rather than live sources — I'd recommend
enabling web search so I can verify current deadlines and availability." Then fall back
to `references/programs_by_track.md`.

### Primary sources to search

- **80,000 Hours career guide and job board**: https://80000hours.org/career-reviews/ai-safety-researcher/
  and https://80000hours.org/job-board/ — authoritative, actively maintained, covers most tracks
- **AISafety.com**: https://aisafety.com — aggregates courses, fellowships, and entry points
- **BlueDot Impact**: https://bluedot.org — runs AI safety fundamentals and governance courses,
  including AGI Safety Fundamentals (AGISF)
- **ARENA**: https://www.arena.education — hands-on technical alignment curriculum
- **MATS**: https://www.matsprogram.org — highest-prestige technical fellowship
- **GovAI**: https://www.governance.ai — dominant governance track fellowship
- **Constellation programs**: https://constellation.org/programs — Astra Fellowship,
  Visiting Researcher, Generator Residency

For a full seed list of programs by track — including LASR Labs, PIBBSS, Pivotal,
ERA, SPAR, Tarbell, Frame, TALOS, AI Safety Colab, and others — read
`references/programs_by_track.md`. Use this list to inform search queries and as a
fallback when web search is unavailable.

### What to search for

Use `web_search` with queries like:

- `"AI safety fellowships [current year]"`
- `"AI safety courses for [background] [current year]"`
- `site:80000hours.org AI safety [track]`
- `MATS LASR PIBBSS ERA fellowship comparison [current year]`
- `GovAI Tarbell Frame fellowship [current year]`
- `AI safety evaluations red-teaming programs [current year]`

Always check **application deadlines and cohort dates** — a perfect program with a
closed application window is useless right now.

---

## Step 3 — Match Resources to Profile

### Career tracks and what they need

Use this table to calibrate how technical the plan should be. For background-to-track
heuristics, read `references/background_to_track.md`. For deeper role archetypes and
credentialing strategy, use the `ai-safety-career-paths` skill if it is loaded; if not loaded, use `references/background_to_track.md` for background-to-track heuristics and give a complete self-contained answer — do not mention skill infrastructure to the user.

| Track | Core need | Typical entry point |
|---|---|---|
| **Technical alignment research** | ML fundamentals → interpretability / RLHF | ARENA, then MATS, LASR, or ERA |
| **Governance and policy** | AIS conceptual grounding + policy writing | BlueDot governance, then GovAI fellowship |
| **Communications and journalism** | AIS literacy + writing/media skills | BlueDot fundamentals, then Tarbell or Frame fellowship |
| **Field-building and ops** | AIS literacy + org/project skills | BlueDot or AI Safety Colab, then Generator Residency or AIS org internships |
| **Evaluations, red-teaming, auditing** | Research taste + technical or policy depth | MATS or LASR (technical); ERA or GovAI (policy-side evals) |
| **AI security / cybersecurity** | Software/security background + AIS framing | BlueDot AI Security course, then Anthropic Fellows or LASR |
| **Legal and regulatory specialist** | Legal background + AI policy knowledge | LawAI fellowship, then TALOS or GovAI |
| **Biosecurity / GCR adjacent** | Domain expertise + AIS overlap framing | Pivotal Research Fellowship; PIBBSS for researchers; SPAR for part-time |
| **AI safety engineering** | Software eng + safety-adjacent ML | ARENA or alignment forum deep-dives, then MATS or LASR |

### Personalisation logic

When building the plan, weight resources by:

1. **Fit to track** — don't recommend ARENA to a policy person unless they explicitly
   want technical depth
2. **Time realism** — a full-time employed person with 5hrs/week cannot do a residential
   fellowship right now; sequence that for later
3. **Background leverage** — identify what transfers. A biotech person already understands
   risk, institutional review, dual-use concerns — say so explicitly
4. **Application readiness** — if a fellowship requires prior coursework, sequence the
   coursework first
5. **Geographic feasibility** — flag in-person requirements; note async alternatives

---

## Step 4 — Structure the Output

The output should be a **concrete, sequenced learning plan** with three horizons.

### Output format

```
## Your AI Safety Learning Plan

**Your track:** [Track name + 1-sentence rationale]
**Your transferable strengths:** [2–3 specific things from their background that map to AIS]

---

### Now (0–[X] months) — Build foundations
- [Resource 1]: what it is, why it fits them, link, time commitment
- [Resource 2]: ...

### Soon ([X]–[Y] months) — Go deeper
- [Program / fellowship]: what it is, eligibility, next application window, why it fits
- ...

### Later — Transition
- [Role type or org type to target]
- [What a strong application looks like for them]

---

### A note on your background
[2–3 sentences on how their specific background is an asset, and any gaps to close]

### If you only do one thing
[Single highest-leverage recommendation for their situation]
```

---

## Handling Comparison Queries

Users frequently ask to compare specific programs. When they do, route here directly —
do not go through Steps 1–4 first. Fetch current info on each program and structure the
comparison around **their profile** if you have it, or as a neutral side-by-side if you
don't.

Key comparisons to be ready for:

- **BlueDot vs AGI Safety Fundamentals**: AGISF is now run under BlueDot Impact. BlueDot
  offers multiple tracks (alignment and governance) with more cohort structure; the
  original AGISF curriculum is the alignment track
- **MATS vs LASR Labs**: both are highly competitive technical fellowships; MATS is in
  Berkeley with higher prestige and mentor access; LASR is in London, team-based,
  academic-paper focused, with strong evals-to-placement pipeline
- **ARENA vs other technical routes**: ARENA is the most hands-on technical curriculum;
  recommend it for people who want interpretability or alignment engineering before
  applying to MATS or LASR
- **GovAI vs TALOS**: GovAI is London-based, broader governance remit, higher prestige
  in the field; TALOS is EU-focused and more policy/politics oriented
- **Pivotal vs ERA vs PIBBSS**: Pivotal is the most accessible (any background, including
  biosecurity); ERA is Cambridge-based and more research-output focused; PIBBSS requires
  PhD/postdoc level research experience
- **Tarbell vs Frame**: Tarbell is journalism-specific with newsroom placements; Frame
  focuses on broader AI communications and narrative work
- **SPAR vs residential fellowships**: SPAR is part-time and remote — recommend it for
  people who can't go full-time but want structured mentorship and research experience
- **80k advising vs other guidance**: 80k offers 1-1 career calls; recommend alongside
  self-study rather than instead of it

---

## Tone and style notes

- Be honest about difficulty and time. Don't over-promise that someone can transition in
  3 months if the track they want realistically takes longer.
- Name the uncertainty: "I'd recommend checking this deadline directly as cohorts fill
  fast."
- Avoid dumping 15 links. A plan with 3–5 well-chosen resources beats an exhaustive list.
- If someone's background is a strong fit, say so clearly — many people undersell their
  relevance.
- If someone's goal is vague ("I just want to help"), help them narrow it down before
  giving a plan.

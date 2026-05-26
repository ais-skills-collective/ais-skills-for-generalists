# AIS Source Registry

An allowlist of sources permitted for verifying AI-safety claims. Used by the
`ai-safety-101` skill. See `../SKILL.md` for how it is applied.

## About this file

Verified in May 2026 and can be updated over time. Where a source publishes versioned documents (RSPs, frontier safety frameworks, etc.), always read the current live version — dated breadcrumbs in entries below record what was current at verification time and are tripwires for detecting drift, not facts to quote.

Tiers:
- **PRIMARY** — papers, official organizational documents, regulatory texts. Win on
  conflict.
- **SECONDARY** — community and commentary sources. Context only; never override a
  primary source.

This ordering resolves *factual* conflicts only — which source is right about what a
document says or what happened. It does **not** apply to contested or evaluative
questions. There, see `perspectives.md`: represent the range of camps and attribute
them; do not let an interested primary source "win" a question of judgment.

---

## Primary

### arXiv
- URL: https://arxiv.org (sections cs.AI, cs.LG, cs.CL)
- Authoritative for: the text of a preprint itself — the claims, methods, and results
  as the authors stated them.
- NOT authoritative for: peer-review status, replication, or acceptance by the field.
- How to query: search arxiv.org or Google Scholar; cite the specific arXiv ID and
  version (e.g. arXiv:2401.00001v2).
- last_verified: 2026-05-21

### Anthropic — research and policy
- URL: https://www.anthropic.com/research , https://www.anthropic.com/news
- RSP URL: https://www.anthropic.com/responsible-scaling-policy
- Authoritative for: Anthropic's own published research and its Responsible Scaling
  Policy (RSP).
- Notes: the RSP is versioned and revised periodically; read the live page.
- last_verified: 2026-05-21

### Google DeepMind — research and safety
- URL: https://deepmind.google/responsibility-and-safety/ , https://deepmind.google/research/
- Authoritative for: DeepMind's published research and its Frontier Safety Framework.
- Notes: the Frontier Safety Framework is versioned and revised periodically; read the live page.
- last_verified: 2026-05-21

### OpenAI — research and safety
- URL: https://openai.com/safety/ , https://openai.com/research
- Authoritative for: OpenAI's published research and its Preparedness Framework.
- Notes: the Preparedness Framework is updated less frequently than the Anthropic and DeepMind frameworks; read the live page for the current version.
- last_verified: 2026-05-21

### METR (Model Evaluation and Threat Research)
- URL: https://metr.org , blog at https://metr.org/blog
- Authoritative for: dangerous-capability evaluation methodology and METR's own
  evaluation reports and benchmarks.
- last_verified: 2026-05-21

### Apollo Research
- URL: https://www.apolloresearch.ai (research: https://www.apolloresearch.ai/science/)
- Authoritative for: Apollo's own evaluation methodology and reports — particularly
  on deceptive alignment, scheming, strategic deception, and evaluation awareness in
  frontier models. It runs pre-deployment evaluations for major labs.
- Notes: a Public Benefit Corporation focused on auditing high-risk failure modes.
  Like METR, authoritative for its own published evaluations, not for field
  consensus.
- last_verified: 2026-05-21

### CAISI — Center for AI Standards and Innovation (US, at NIST)
- URL: https://www.nist.gov/caisi
- Authoritative for: CAISI's published AI model evaluations and standards work.
- Notes: this body was the US AI Safety Institute until June 2025, when it was
  renamed CAISI and re-oriented toward national-security risks (cyber, biosecurity,
  chemical) and "pro-innovation" standards. The word "safety" was dropped. Treat its
  remit as security/standards-focused, not broad AI safety.
- last_verified: 2026-05-21

### UK AI Security Institute
- URL: https://www.aisi.gov.uk
- Authoritative for: the UK institute's model evaluations and published reports.
- Notes: renamed from "AI Safety Institute" to "AI Security Institute" in February
  2025, with a remit shift toward national-security and criminal-misuse risks and
  away from ethics/bias topics. Scope its authority accordingly.
- last_verified: 2026-05-21

### EU AI Act — official texts
- URL: https://eur-lex.europa.eu (legal text) ,
  https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai ,
  https://ai-act-service-desk.ec.europa.eu (official implementation desk)
- Authoritative for: the legal text of the EU AI Act and official implementation
  timelines.
- Notes: obligations phase in on staggered deadlines (a major tranche applies
  2026-08-02). The deadlines are themselves in flux — the EU has moved to amend
  rules and extend some deadlines — so always check the current official timeline.
- last_verified: 2026-05-21

### NIST — AI Risk Management Framework
- URL: https://www.nist.gov/itl/ai-risk-management-framework
- Authoritative for: the text of the NIST AI RMF and its associated profiles.
- last_verified: 2026-05-21

### International AI Safety Report
- URL: https://internationalaisafetyreport.org (full report and the Extended Summary
  for Policymakers)
- Authoritative for: a consensus scientific synthesis of general-purpose AI
  capabilities, risks, and mitigations. Chaired by Yoshua Bengio and written by 100+
  experts with 30+ governments and international bodies backing it, it is explicitly
  built to represent the *range* of expert views, including where they disagree —
  the best single source for "what the field as a whole concludes."
- Notes: published annually; the 2026 edition (second iteration) appeared February
  2026. Cite the edition and date. Not a substitute for a primary research paper on
  a specific result — use it for synthesis and the spread of expert opinion.
- last_verified: 2026-05-21

---

## Secondary

### 80,000 Hours
- URL: https://80000hours.org (problem profiles: https://80000hours.org/problem-profiles/; career reviews: https://80000hours.org/career-reviews/)
- Use for: 80k's own stated positions — its published problem profiles (including "Risks from power-seeking AI systems"), career reviews, and strategic framing of AI risk. Authoritative for what 80k argues; not authoritative for empirical claims or field consensus.
- Caution: 80k is an effective-altruism-adjacent advocacy organisation, not a research body. Its framing reflects its own priorities. When citing, attribute to 80,000 Hours specifically, not "the field."
- last_verified: 2026-05-25

### Alignment Forum
- URL: https://www.alignmentforum.org
- Use for: technical alignment discussion and researchers' informal write-ups.
- Caution: not peer-reviewed; quality varies; a post represents its author's view,
  not field consensus.
- last_verified: 2026-05-21

### MIRI / Yudkowsky primary writings
- URL: https://intelligence.org (publications: https://intelligence.org/all-publications/) ;
  Eliezer Yudkowsky's posts on https://www.lesswrong.com and https://www.alignmentforum.org
- Use for: the stated positions and arguments of MIRI and of Eliezer Yudkowsky —
  i.e. verifying an attributed claim ("Yudkowsky argues X", "MIRI's position is Y")
  or the framing of a concept as originally set out in their writing.
- NOT authoritative for: empirical claims, field consensus, or whether a position is
  correct. This is one organization's perspective, and an unusually strong-position
  one.
- Scope note: MIRI pivoted around 2024 from technical alignment research toward
  policy advocacy aimed at halting or restricting frontier AI development.
  Distinguish older technical work from current governance/advocacy output, and date
  what you cite.
- last_verified: 2026-05-21

### Arbital (alignment content, archived on LessWrong)
- URL: https://www.lesswrong.com/w/eliezer-s-lost-alignment-articles-the-arbital-sequence
  (import note: https://www.lesswrong.com/posts/fwSnz5oNnq8HxQjTL/arbital-has-been-imported-to-lesswrong)
- Use for: detailed explainer-style treatments of alignment concepts (e.g.
  corrigibility, pivotal act, instrumental convergence) written ~2015-2017 by
  Yudkowsky, Soares, Christiano and others.
- Notes: the Arbital platform was discontinued in 2017; its public content was
  migrated to LessWrong (read-only) in collaboration with MIRI. Do not cite
  arbital.com — it is defunct.
- Caution: this is preserved 2015-2017 material, not maintained. A framing here may
  be the origin of a term without being its current usage — date it and cross-check
  against current sources.
- last_verified: 2026-05-21

### Epoch AI
- URL: https://epoch.ai (data and benchmarks) , https://epochai.substack.com (blog)
- Use for: quantitative trends in compute, scaling, model performance, and
  benchmark data (including the Epoch Capabilities Index).
- Caution: confirm the methodology and date attached to each figure.
- last_verified: 2026-05-21

### Lab engineering and safety blogs
- URLs: the official blogs linked from anthropic.com, openai.com, and
  deepmind.google.
- Use for: context and announcements. For any policy or framework claim, cite the
  official document, not the blog post about it.
- last_verified: 2026-05-21

---

## Limited use — routine facts only

Reputable, established news organizations (those with editorial standards and a
corrections process) may be cited for **routine, uncontroversial facts** — who leads
an organization, that an agreement was signed, basic organizational or biographical
detail. Label them as secondary. Do **not** use them for quantitative claims,
contested research results, or fine-grained attributed positions — those need a
primary source or must not be asserted.

## Never cite

General web-search result pages, social-media posts, AI-generated summaries, and
Wikipedia (Wikipedia may be used to *find* a primary source, never cited as one). A
personal blog is not authoritative unless its author is the primary researcher and
the post is itself the original source of the claim.

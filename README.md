# AI Safety Skills for Generalists

A suite of Claude skills to help generalists explore, learn about, and pivot into AI safety.

## What this is

AI safety needs more generalists: programme managers, field-builders, operators, org leaders, chiefs of staff, founders. But the pathways for them to identify relevant opportunities, leverage existing skills, upskill, and build credentials are not well established. We've built a suite of Claude skills that combine the scattered AI safety career resources with the intelligence of Claude to help generalists find better guidance into the field. Each skill gives Claude reliable, current grounding in a different piece of the pivot puzzle — the field itself, how your skills map onto it, how to upskill, and how to fund the work. Install the skills, and Claude becomes a substantially more useful guide in your journey into AI safety.

Skills follow the [Anthropic Agent Skills format](https://support.claude.com/en/articles/12512198) — folders containing a `SKILL.md` and supporting reference material that Claude loads on demand. They work in claude.ai (Free, Pro, Max, Team, and Enterprise plans), Claude Code, and via the API.

## Who this is for

You're a mid-career professional, most likely from a non-technical background — communications, policy, law, journalism, consulting, product, operations, research, strategy. You've been hearing about AI safety, you know it matters, and you want to understand the field well enough to figure out whether and how you might contribute to it.

The pivot questions you're trying to answer probably include some or all of:

- What is AI safety actually about, and which parts of it match my interests?
- Is my existing background useful in AI Safety, or do I need to retrain from scratch?
- If I want to upskill, where do I start, and how long does it take?
- How do people fund this kind of work — for projects, for transitions, for independent research?

These skills are aimed at exactly those questions.

## The skills at a glance

| Skill | What it is | When to use it |
|---|---|---|
| **AI Safety 101** | Orientation in the field — concepts, subfields, key organisations, talent needs | You want to move from vague interest to an informed sense of the landscape |
| **AI Safety Career Paths** | A mapping of your existing skills onto realistic AI safety roles | You're trying to identify where your background and skills actually fit |
| **AI Safety Learning Paths** | Personalised guidance on courses, fellowships, and self-study | You've picked a direction and want a concrete upskilling plan |
| **AI Safety Funding** | A guide to funding for projects, independent research, and career transitions | You have something — a project, an initiative, a transition plan — that needs financial support |

*These skills are designed to work together. Most pivot journeys touch all four areas — orientation, career mapping, learning, and (often) funding. **Install all four**, even if some feel less immediately relevant. They'll come into play as your pivot progresses.*

## The skills in detail

### AI Safety 101

Builds accurate, structured context on what AI safety is, what it isn't, and how the field is organised. Without this baseline, the rest of the pivot is guesswork — you can't choose a path through a field you don't yet have a map of. The skill covers foundational concepts (alignment, interpretability, governance, evaluations), the main subfields and how they connect, the key organisations and people, current debates, and the misconceptions newcomers most often arrive with.

**Sample queries**

> *"What is AI safety actually about? I keep seeing the term but I can't tell if it's a technical field, a policy field, or both."*
>
> *"How is AI safety different from AI ethics, AI alignment, and responsible AI? These all seem to blur into each other."*
>
> *"Give me a quick map of the AI safety field — the main subfields, what kind of work happens in each, and how they connect."*
>
> *"Who are the key organisations and people I should know about to get oriented in AI safety?"*

&nbsp;

### AI Safety Career Paths

Translates your existing professional skills into AI safety roles you might realistically hold. Most generalists rule themselves out of AI safety unnecessarily. The skill covers the full spectrum of generalist roles (well beyond technical research), what specific orgs hire for, and how to translate skills like writing, project management, policy analysis, research, or operations into AI safety terms.

**Sample queries**

> *"I'm a journalist with 8 years' experience. What roles in AI safety would actually use my skills?"*
>
> *"For someone early in their career coming from a non-AI-safety background with experience in community building, what opportunities exists in operations or field-building AI safety role'?"*
>
> *"Do I need to be technical to work in AI safety? If so, how technical, and what can a non-technical generalist do instead?"*
>
> *"I'm a senior PM in a non-AI company. What does an AI safety pivot look like for someone at my level?"*

&nbsp;

### AI Safety Learning Paths

Helps identify a personalised upskilling plan based on your goals and current skills. The AI safety learning landscape is full of programmes — BlueDot, ML4Good, ARENA, and many more — and it's not obvious which ones fit which background, in which order, with what time commitment. The skill covers the major courses and fellowships, how to choose between them based on your goals and constraints, reading lists and sequencing, and how to make progress alongside a full-time job.

**Sample queries**

> *"I've decided I want to work in AI safety communications. What should I learn, and in what order?"*
>
> *"I'm a biotech researcher considering a pivot into AI safety. What course or fellowship should I consider to upskill myself for the right opportunities?"*
>
> *"I'm trying to choose between BlueDot Technical AI Safety and ARENA programmes. Which one fits someone with my background?"*
>
> *"I have about 6 months of evenings and weekends to upskill. Suggest a realistic learning plan to build my fundamental skills in AI governance."*

&nbsp;

### AI Safety Funding

Maps the funding landscape so you can find sources that fit what you're trying to do, and understand which funders to focus on. The skill covers speculative grants, strategic grantmakers, career-transition funds, incubators, safety-aligned VC, government programmes, individual donors, and prizes. It addresses application processes, realistic raise amounts, and which funders fit which kinds of projects.

**Sample queries**

> *"I'm working on an AI safety communications project. Who would realistically fund something like this?"*
>
> *"Which funders support early-stage or speculative AI safety research projects? I don't have a track record yet."*
>
> *"I'm thinking of leaving my job to retrain into AI safety. Are there funders that support career transitions?"*

## Installation

### In claude.ai

> [!NOTE]
> **Prerequisites.** Skills work on all Claude plans, including the free tier. Before you can upload skills, you need **Code execution and file creation** enabled. Go to **Settings → Capabilities** and toggle it on. On Team or Enterprise plans, this setting may be managed by an administrator — check with them if the toggle isn't available.

1. In Claude sidebar, go to **Customize → Skills**.
2. Download the skill zips from the [latest release](https://github.com/ais-skills-collective/ais-skills-for-generalists/releases/latest):
   - `ai-safety-101.zip`
   - `ai-safety-career-pathfinder.zip`
   - `ai-safety-learning-path.zip`
   - `ai-safety-funding.zip`
3. Click **+ → Create skill** → Upload skill**, select a zip, and toggle the skill on.
4. Repeat for each skill you want.

Claude activates the relevant skill automatically when your question is in its scope. You can also invoke a skill explicitly using the / command or prompting:

> *"Use the AI Safety Career Paths skill — I'm a journalist with 8 years' experience, what roles would actually use my skills?"*

### Advanced: In Claude Code

For developers using Claude Code from the terminal, add this repo as a plugin marketplace:
Then install all four skills, or pick individual ones via the marketplace UI.

## Updates and versioning

The suite is versioned together using semantic versioning. When skills are updated — new fellowships in the Learning Path, new funders in Funding, refreshed role inventories in the Pathfinder — we cut a new release with a changelog entry explaining what changed.

To get an update, re-download the relevant zips from the latest release and re-upload them in **Customize → Skills**, replacing the older versions. Subscribe to releases on this repo (**Watch → Custom → Releases**) to be notified.

See [CHANGELOG.md](CHANGELOG.md) for release history.

## Limitations

> [!IMPORTANT]
> **Things change fast in AI safety.** Each `SKILL.md` carries a `last-verified` date. For fast-decaying content — open fellowship windows, current funder priorities, role openings — skills instruct Claude to flag the as-of date and suggest verifying at source. The skills are most useful as a current-as-of-X baseline.
>
> **Not a substitute for community.** Skills are an LLM grounding tool. They don't replace mentors, programmes, or the conversations that actually surface roles and funding. They make Claude useful in between those conversations.
>
> **Bias toward generalists.** Skills are built primarily for non-technical pivoters — governance, communications, ops, policy, field-building. Technical pivoters will find them useful, but they don't go deep on the technical research landscape.

## Feedback

If something is outdated, wrong, or missing, please [open an issue](https://github.com/ais-skills-collective/ais-skills-for-generalists/issues/new). Particularly valuable:

- Anything you tried to use a skill for that didn't work as expected
- Content you expected to find and didn't
- Out-of-date references (closed fellowships, retired roles, broken links)

## Contributing

We're not actively soliciting contributions while the suite is in early release. If you want to contribute content or a new skill, please open an issue to discuss before investing time in a PR. See [CONTRIBUTING.md](CONTRIBUTING.md).

## Authors

Built by Alex Borwick, Jaspreet Singh, and Seti Arabshahi. Equal contributors. See [AUTHORS.md](AUTHORS.md).

## License

MIT. See [LICENSE](LICENSE).

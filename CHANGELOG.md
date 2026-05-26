# Changelog

All notable changes to this project will be documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [0.1.0] — 2026-05-26

First public release. Four Claude skills for mid-career professionals pivoting into AI safety.

### Added

- **AI Safety 101** — field orientation skill covering core concepts, motivations, subfield structure, contested questions, and curated reading lists. Designed for people coming to AI safety from adjacent backgrounds (policy, product, ML, journalism, generalist).

- **AI Safety Career Paths** — career mapping skill that translates existing professional backgrounds into realistic AI safety role options across technical, governance, ops, comms, policy, hybrid, and founder paths. Covers 11 professional backgrounds and detailed role archetypes with per-org bar expectations.

- **AI Safety Learning Paths** — personalised learning plan skill covering courses, fellowships, and self-study sequences across all career tracks. Compares programmes including BlueDot, ARENA, MATS, GovAI, AISES, and AGI Safety Fundamentals. Uses web search for live deadlines and cohort status.

- **AI Safety Funding** — funding navigation skill covering the full landscape: speculative grants, strategic grantmakers, career-transition funds, incubators, safety-aligned VC, government programmes, prizes, and RFPs. Includes light pitch review and funder shortlisting matched to project shape and ask size.

- GitHub Actions release workflow — automatically builds per-skill zips on tag push and attaches them as release assets in the correct format for claude.ai upload.

### Notes

- Skills are designed to work standalone or as a suite. Each skill degrades gracefully when adjacent skills are not installed — routing instructions include explicit fallbacks so users never hit a dead end.
- All skills follow the Anthropic Agent Skills format and are installable via claude.ai (all plans including free) by uploading the zip to a Project.
- Content is current as of May 2026. Fast-moving content (fellowship deadlines, funder priorities) is flagged within skills with "verify at source" prompts.

[0.1.0]: https://github.com/ais-skills-collective/ais-skills-for-generalists/releases/tag/v0.1.0
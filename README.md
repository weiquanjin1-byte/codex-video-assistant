# codex-video-assistant

[![Release](https://img.shields.io/github/v/release/weiquanjin1-byte/codex-video-assistant?display_name=tag)](https://github.com/weiquanjin1-byte/codex-video-assistant/releases/tag/v0.1.0)

An open workflow project for training Codex into a learning, planning, reviewing, and compliance-aware AI video editing assistant.

## Project Status

Initial open source release completed.

Current release: [v0.1.0 - Initial Open Source Release](https://github.com/weiquanjin1-byte/codex-video-assistant/releases/tag/v0.1.0)

This public repository contains workflow documentation, agent definitions, skills, examples, an aesthetic scoring rubric, and compliance guidance. It does not include private media assets, platform credentials, internal learning records, API keys, tokens, cookies, account data, or unpublished production materials.

## What Problem This Solves

Short video production is not only about generating a script. A usable assistant needs to connect topic research, script writing, captions, voice style, BGM direction, editing rhythm, aesthetic review, and copyright checks.

`codex-video-assistant` provides a structured project system for building that assistant with:

- Codex autonomous learning records
- Multi-agent collaboration
- Video editing workflow templates
- Aesthetic scoring
- Compliance and source review
- Reusable Skill instructions
- Offline and online operating modes

## Core Capabilities

| Capability | Description |
|---|---|
| Autonomous learning | Records what Codex learns, why it matters, and how it maps to project goals. |
| Source review | Tracks whether sources are public, reliable, relevant, and suitable for use. |
| Multi-agent workflow | Splits video work into trend research, script, copywriting, voice, BGM, editing, aesthetic review, and compliance review. |
| Video planning | Produces briefs, scripts, storyboard tables, timeline drafts, subtitle plans, and production checklists. |
| Aesthetic scoring | Reviews rhythm, narrative clarity, visuals, captions, voice, BGM, emotion, platform fit, and conversion intent. |
| Compliance review | Checks privacy, copyright, plagiarism, hallucination, platform rules, and licensing status. |
| Skill mechanism | Turns repeated project actions into reusable instructions under `skills/`. |

## Multi-Agent Architecture

The project uses eight agents:

1. `trend-research-agent` finds public, authorized, or user-provided topic signals.
2. `script-writing-agent` turns a topic into a video position, hook, script, and storyboard.
3. `copywriting-agent` writes titles, covers, post copy, hashtags, and platform-specific variants.
4. `voice-selection-agent` chooses voice style, pace, emotion, pauses, and emphasis.
5. `bgm-selection-agent` chooses BGM mood, style, BPM, volume, and authorization status.
6. `editing-plan-agent` creates the timeline, shots, captions, transitions, export specs, and minimum production steps.
7. `aesthetic-review-agent` scores and improves the plan using `aesthetic-score.md`.
8. `compliance-review-agent` performs the final privacy, copyright, licensing, plagiarism, and hallucination review.

See [docs/multi-agent-architecture.md](docs/multi-agent-architecture.md).

## Skills

Skills are reusable workflow instructions. This project currently includes:

- `skills/video-content-workflow/SKILL.md`: video planning, aesthetic scoring, source checks, and multi-agent execution rules.

See [skills/README.md](skills/README.md).

## Video Production Workflow

The default workflow is:

1. Define platform, audience, duration, video type, and goal.
2. Review public or user-provided sources.
3. Build the script structure: hook, body, turn, ending.
4. Convert script paragraphs into storyboard shots.
5. Plan captions, voice style, BGM direction, and editing rhythm.
6. Check material, BGM, font, sound effect, voice, and image rights.
7. Score the plan with the aesthetic scoring system.
8. Improve the plan.
9. Run final compliance review before production or publication.

See [docs/workflow.md](docs/workflow.md).

## Aesthetic Scoring System

The project uses a 100-point review system covering:

- Opening attraction
- Narrative clarity
- Editing rhythm
- Visual continuity
- Caption readability
- Voice match
- BGM match
- Emotional consistency
- Platform fit
- Conversion guidance

The detailed rubric is in `aesthetic-score.md`.

## Compliance And Copyright Statement

This project does not provide permission to use copyrighted materials. Before using any BGM, video, image, font, sound effect, icon, voice, or likeness, you must confirm authorization and usage rights.

Trend research may only use public, authorized, or user-provided data sources. The project must not bypass platform restrictions, collect private information, or fabricate popularity data.

This project is an assistant for creative planning and review. It does not guarantee that generated content is suitable, lawful, high-performing, or publishable.

See [docs/compliance.md](docs/compliance.md).

## Offline And Online Modes

### Offline Mode

Use offline mode when you want privacy-first planning without internet access.

Offline mode can:

- Generate briefs, scripts, storyboards, captions, and editing plans from user input
- Run aesthetic scoring
- Run compliance checklists
- Mark unknown source or license items as `pending manual confirmation`

Offline mode cannot:

- Verify current platform trends
- Confirm live GitHub, website, or license changes
- Confirm whether a specific song, font, image, or voice is authorized

### Online Mode

Use online mode only when you have compliant access to public or authorized sources.

Online mode can:

- Check public project documentation
- Review open-source project metadata
- Record source URLs and licenses
- Compare public references

Online mode must not:

- Bypass platform restrictions
- Scrape private or restricted data
- Use cookies, tokens, private accounts, or private messages without authorization
- Claim unverifiable trend data as fact

## Quick Start

1. Clone or copy the project.
2. Read `PROJECT.md` to understand the project goal and boundaries.
3. Read `docs/getting-started.md`.
4. Choose a video topic or brief.
5. Follow `docs/workflow.md` or `agents/README.md`.
6. Save only public-safe examples in `examples/`.
7. Keep private evidence, keys, account data, and unpublished materials out of the public repository.

## Project Roadmap

- Stage 1: Project learning and source review system
- Stage 2: Video production workflow
- Stage 3: Multi-agent collaboration
- Stage 4: Aesthetic scoring and optimization
- Stage 5: Compliance review and publishing safety
- Stage 6: Optional automation for script, subtitle, and video prototype generation

## Current Limitations

- The project does not automatically bypass or scrape platforms.
- The project currently does not provide automatic platform trend crawling. Trend research only supports public, authorized, or user-provided data sources.
- The project does not include licensed BGM, fonts, stock videos, voice assets, or icons.
- The project does not guarantee that a generated video plan is suitable for publication.
- Trend, license, and platform rule checks may require manual verification.
- Evidence files may contain private work records and should be reviewed before publishing.

## Repository Safety

The initial public release intentionally excludes:

- Internal learning records
- Raw task evidence
- Reports and private project logs
- Platform cookies, tokens, API keys, and credentials
- Private or unlicensed video, image, audio, subtitle, font, icon, BGM, voice, or production assets

## Disclaimer

This project is for planning, learning, and workflow assistance. It is not legal advice, copyright advice, platform policy advice, or a guarantee of content performance. Users are responsible for verifying rights, licenses, facts, privacy compliance, and platform rules before publishing any content.

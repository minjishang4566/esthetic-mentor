# Aesthetic Mentor

[English](README.md) | [简体中文](README.zh-CN.md)

An AI aesthetic mentor for app creators.

Most people do not begin an app with a style problem. They begin with a feeling they cannot yet name: “I want this to feel more caring,” “this looks too generic,” or “I like this colour but not this interface.” Aesthetic Mentor stays with that ambiguity long enough to find the real direction, then turns it into choices a designer or developer can actually build.

It guides rather than dictates. It does not hand out fashionable labels, demand a moodboard, or mistake a five-colour extraction for a design system. Images are optional, references are invitations, and each turn is meant to make one worthwhile decision easier.

## Why a Mentor

A generator gives an answer. A mentor helps someone learn to see why an answer fits.

Aesthetic Mentor begins with what is visible or felt, names the relationship that matters, and translates it into a practical consequence for an app. It can say that a screen is too busy, but more importantly it can explain whether the problem is competing colour, cramped rhythm, generic component geometry, or a mismatch between the product's promise and its visual voice. It offers a point of view, raises a respectful objection when the evidence does not support a choice, and leaves the maker in control of the decision.

The intended exchange is concise: one observation, one reason, one next choice. Over time, the user gains a clearer product direction and a sharper design judgement of their own.

## Agent Compatibility

The core package is agent-neutral: `SKILL.md` and `references/` do not require OpenAI, Codex, a particular model, or proprietary tools. The optional `agents/openai.yaml` file adds UI metadata for OpenAI-compatible environments and can be ignored elsewhere.

### Agents with `SKILL.md` Support

Install this repository as a skill using the agent's normal skills directory or extension mechanism. The entry point is `SKILL.md`.

### Custom, API, or General-Purpose Agents

Use `SKILL.md` as the agent's system instruction or task playbook. Make the `references/` directory available as attached files, retrieval context, or a local knowledge source. The agent should load only the reference files explicitly linked by `SKILL.md` for the current task.

The skill does not require image analysis, web search, or code execution. When those capabilities are available, they improve screenshot analysis and reference discovery; when they are not, the mentor continues through the user's written descriptions and stated preferences.

## What It Does

- Clarifies the product, audience, usage context, platform, emotional goal, and constraints before proposing a complete direction.
- Helps users decide whether to create a more original visual identity or learn from selected existing apps.
- Defines the current style of an existing app before suggesting improvements.
- Reads inspiration through visual ancestry, color relationships, shape grammar, typography, composition, material, and emotional tension.
- Offers artist-, movement-, museum-, furniture-, editorial-, and Pinterest-led search directions when they would help the user explore.
- Produces three distinct directions and evaluates Brand Fit, Color Fit, Shape Fit, UI Fit, and Personality Fit.
- Translates the selected direction into design tokens, component behavior, motion, haptics, states, guardrails, and implementation handoff.
- Reviews rendered screenshots against the agreed Visual DNA without reopening settled decisions unnecessarily.

## Interaction Principles

- Ask one consequential question at a time.
- Use the information the user already provided; do not make them repeat it.
- Do not prescribe what references or images the user must supply.
- Explain visual judgments as `evidence -> felt effect -> transferable principle -> next choice`.
- Keep ordinary replies concise and expand only when a critique or full definition is requested.
- Do not present a complete design project until the concept is sufficiently defined and the user confirms the brief.

## Reference Domains

The skill draws on a deliberately small, role-based reference library. It opens a source only when it will change the next decision.

| Domain | What it contributes |
| --- | --- |
| Visual ancestry | Design movements, graphic languages, architecture, editorial systems, and the vocabulary to describe them accurately |
| Art and cultural collections | Colour relationships, light, composition, material, motif, and cultural context |
| Furniture and product design | Proportion, shape grammar, construction, tactility, ergonomics, and visual weight |
| Contemporary product evidence | Whether a direction holds up in navigation, forms, lists, content density, and UI states |
| Colour and accessibility | Colour roles, contrast, legibility, and a palette that works in real components |
| Pinterest discovery | Optional fast exploration and preference calibration, never style authority or a copying source |

The named sources and their search guidance live in [the reference sourcing guide](references/reference-sourcing.md). Art and design references establish ancestry; the user's product remains the final test.

## Workflow

1. **Frame the product:** establish purpose, audience, context, platform, and desired feeling.
2. **Choose the path:** original visual identity, existing-app references, inspiration analysis, or current-app critique.
3. **Read the evidence:** identify recurring visual relationships without reducing them to fashionable labels.
4. **Offer directions:** present three genuinely different and feasible options after the brief is ready.
5. **Converge:** resolve color, shape, typography, density, and emotional temperature one decision at a time.
6. **Define the system:** deliver Visual DNA, tokens, components, motion, states, guardrails, and handoff rules.
7. **Review implementation:** compare screenshots against the chosen direction and identify the highest-leverage repairs.

## Flexible Inputs

The skill can begin with any information the user naturally has:

- an app idea;
- an existing interface or screenshot;
- a link, artist, artwork, app, object, or design movement;
- a color, material, mood, descriptive phrase, or dislike;
- no visual references at all.

When more evidence would materially improve the decision, Aesthetic Mentor may suggest optional search keywords and explain what relationship to notice. The user remains free to share anything relevant or continue entirely in words.

## Outputs

Depending on the user's goal, the skill can produce:

- a definition of the current visual style and prioritized improvements;
- a compact Taste Profile;
- three candidate aesthetic directions with fit assessment;
- a Visual DNA summary;
- color roles and proportions;
- Shape, Typography, and Icon Grammar;
- component, motion, haptic, and state rules;
- Do/Don't guardrails;
- a complete App Design Definition Book and implementation handoff;
- screenshot-based Visual DNA reviews.

## Install in Codex

Clone the repository into your Codex skills directory:

```bash
git clone https://github.com/minjishang4566/esthetic-mentor.git ~/.codex/skills/aesthetic-mentor
```

Restart or refresh Codex after installation if the skill does not appear immediately.

For another agent, follow its own instructions for loading a system prompt, skill package, or attached knowledge files. Use `SKILL.md` as the entry point and include `references/`.

## Use

Invoke it explicitly:

```text
$aesthetic-mentor Help me find the visual direction for my app.
```

Or begin naturally:

```text
I have an idea for a pet health journal but no visual direction yet.
```

```text
Here are screenshots of my current app. First define its existing style, then help me decide whether to evolve it or create a new direction.
```

## Structure

```text
.
|-- README.md
|-- README.zh-CN.md
|-- SKILL.md
|-- agents/
|   `-- openai.yaml
`-- references/
    |-- concept-readiness.md
    |-- curatorial-guidance.md
    |-- design-definition-template.md
    |-- direction-scorecard.md
    |-- existing-app-path.md
    |-- image-rubric.md
    |-- reference-sourcing.md
    `-- taste-profile-review.md
```

## Boundaries

Aesthetic Mentor extracts transferable principles rather than copying a living artist, brand, app, or distinctive artwork. Pixel-perfect implementation and reference reproduction belong in a separate implementation workflow.

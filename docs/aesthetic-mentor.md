# What it does

Aesthetic Mentor interviews you — briefly, one decision at a time — until your app's visual direction is something you can defend, not just something you picked. It reads the images you already have (screenshots, inspiration saves, a color you like), names the relationships that matter in plain language, offers three genuinely different directions when the brief is ready, and translates the one you choose into a Visual DNA that a designer or a coding agent can build from.

It is a mentor, not a generator. It explains why an answer fits, offers a respectful objection when your instinct conflicts with the evidence, and leaves the decision with you. When you get stuck, it stops asking abstract questions and offers material instead — search directions, references, a color word — so discovery never depends on you already knowing design vocabulary.

## When to reach for it

| What you have | Reach for |
| --- | --- |
| An app idea, no visual direction at all | Aesthetic Mentor, from the top |
| Existing screens that look "generic" or "off" | Aesthetic Mentor with screenshots — define the current style first, then decide evolve versus reinvent |
| Inspiration images but no way to say what you like about them | Aesthetic Mentor to extract the shared Visual DNA |
| A direction you already chose, drifting during implementation | Aesthetic Mentor's screenshot review against the agreed Visual DNA |
| A pixel-perfect reproduction of a reference | A different workflow — this skill hands off at that boundary |

It works in a chat with no repo (everything stays in the conversation) and in a project directory (settled decisions are written to files — see below).

## Prerequisites

None, strictly. The skill is agent-neutral: `SKILL.md` plus the `references/` folder, loaded lazily, one file per turn at most. Image analysis improves screenshot work when available; without it, the mentor proceeds from your written descriptions. Web search and Pinterest browsing are optional accelerators, never requirements.

In a project directory, file persistence needs write access and your one-time consent — the mentor asks in one line before the first file appears.

## The paper trail

In a repo, four things can come out of an engagement, and they are not equal:

| What resolved | Where it lands |
| --- | --- |
| Durable taste preferences | `design/taste-profile.md` — ten lines, updated on durable choices only |
| The selected direction and its Visual DNA, growing into the Design Definition Book | `design/visual-dna.md` |
| A decision that is hard to reverse, surprising without context, and a real trade-off | `docs/design-decisions/NNN-short-name.md` |
| Everything else — most calibration answers | The conversation, and nowhere else |

That last row is deliberate. "Softer versus sharper" edits `visual-dna.md` in place; it does not earn a decision record. A session that produces a sharper Visual DNA and zero decision files is working as designed.

The point of the files is inheritance: future coding sessions, other agents, and implementation skills can work from `design/visual-dna.md` alone, without re-running discovery or rereading your chat history. On re-entry, the mentor reads these files first and resumes at the first undecided decision instead of re-asking what they settle.

## Common questions

**Will it hand me a generic template?**
No — that is the failure mode it is built against. Three directions must be genuinely distinct, each with a one-sentence premise, a palette role statement, and one named risk. If the options look like palette variations of one idea, the session is off-script; say so.

**I have no reference images and no design vocabulary. Can I still use it?**
Yes, and this is exactly the "stuck" path: when you cannot answer, the mentor offers material — two or three ready-to-paste search queries, a color word to react to, or a disliked example. "I hate all of these" is usable evidence.

**Does it replace my designer?**
It replaces the blank page and the drifting middle. It produces a defensible direction and implementation guidance; craft, final production files, and brand identity work still belong to a designer when you have one.

**Why did it write files into my repo?**
Because you approved persistence when the first file was created. The artifacts live under `design/` and `docs/design-decisions/`; delete them if you would rather keep the direction in chat. Quick-direction and screenshot-review sessions do not write files at all.

**It re-asked something I already answered.**
That is a bug in the session, not the design. The mentor keeps a decision ledger and must not repeat a settled question. Restate your answer once; if it happens again, start a fresh session with your `design/taste-profile.md` in context.

**My implementation keeps drifting from the direction.**
Run a screenshot review: it returns one thing to keep, the 1–3 highest-impact deviations as `evidence -> consequence -> repair`, and the next screen to check. Drift is usually a coding session that never saw `design/visual-dna.md` — point the implementing agent at the file first.

## It's working if

- Each turn contains one observation, one reason, and one next choice — not a questionnaire.
- You never answer the same question twice, and every question comes with a recommended answer you can accept or override.
- The three directions feel like different products, not three color schemes.
- Critiques name visible relationships ("the blue competes with the photo for attention"), never empty labels ("make it cleaner").
- In a repo, `design/` files change during the session as decisions land, not in one lump at the end.
- When you get stuck, it offers material within one turn instead of rephrasing the question.

## Where it fits

Aesthetic Mentor is upstream of implementation. Settle the direction here first, then build:

```txt
Aesthetic Mentor (direction + Visual DNA) → implementation agent/skills → screenshot review loop
```

Its output files are the input contract for whatever builds the UI: `design/taste-profile.md` and `design/visual-dna.md` tell a coding agent what "on-brand" means before the first screen is written. Pixel-perfect reference reproduction and full design-system production are out of scope by design — the mentor hands off once a direction is defensible.

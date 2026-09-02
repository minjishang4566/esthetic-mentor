# Repository Persistence Format

Load only when creating or updating repository artifacts. Files are created lazily at the first resolution, updated the moment a decision lands, and kept short enough to read in one pass.

## File Layout

```text
<project root>/
├── design/
│   ├── taste-profile.md
│   └── visual-dna.md
└── docs/
    └── design-decisions/
        ├── 001-quiet-canvas-with-single-blue-accent.md
        └── 002-editorial-type-over-system-type.md
```

If the project already keeps design docs under another convention (for example a `DESIGN.md` at the root, or an existing `docs/design/` folder), follow that convention instead of imposing this one. Never duplicate: one fact lives in one file.

## design/taste-profile.md

The Taste Profile exactly as defined in [the calibration and review guide](taste-profile-review.md): ten lines or fewer, updated only on durable choices. This file is the first one created, because it starts accumulating before a direction exists.

## design/visual-dna.md

Start from sections 1–2 of [the definition and handoff template](design-definition-template.md) (Direction in One Screen + Visual DNA) the moment a direction is selected. Add sections 3–5 (tokens, components, motion/states, guardrails) as they stabilize. The finished file is the Design Definition Book; do not create a second, parallel document.

Keep the working name and north-star feeling at the top so a future session can re-orient in five seconds.

## docs/design-decisions/NNN-short-name.md

Write a decision record only when all three gates pass:

1. **Hard to reverse**: the cost of changing this later is a rework of shipped surfaces, not a token edit.
2. **Surprising without context**: a future contributor will wonder why the direction is this way.
3. **A real trade-off**: genuine alternatives existed and one was chosen for stated reasons.

Most calibration answers fail gate three; they belong in `design/visual-dna.md`, not here. A session that ends with zero decision records is working as designed.

```markdown
# NNN. [Decision in one sentence]

**Status:** chosen

**Context:** [The tension, and the alternatives that were genuinely considered.]

**Decision:** [What was chosen, stated as a visible rule someone can check in the UI.]

**Consequence:** [What this constrains or costs later, honestly.]
```

## Update Discipline

- Write the moment a decision lands; never batch updates to the end of a session.
- When a new decision contradicts what a file says, surface the conflict in one sentence, resolve it with the user, then write. Do not silently overwrite.
- Trim or split a file rather than let it accumulate; artifacts that no one rereads have failed their job.
- These files are the handoff: future coding sessions, implementation skills, and other contributors should be able to work from them alone.

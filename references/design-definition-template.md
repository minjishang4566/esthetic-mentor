# Design Definition Book and Handoff Template

Create this only after a direction has been selected or explicitly requested. Keep the top section readable by a founder; make the bottom section usable by a designer or developer.

## 1. Direction in One Screen

```markdown
# [Product] Visual Direction: [Working Name]
**North-star feeling:** [3–6 words]
**Visual ancestry:** [layout influence] + [personality influence] + [optional material/editorial influence]
**Core tension:** [e.g. structured, never cold]
**Design promise:** [one sentence]
```

## 2. Visual DNA

```markdown
## Color Roles
| Role | Token name | Value/range | Target share | Job |
| --- | --- | --- | ---: | --- |
| Canvas | color.canvas | ... | 55–70% | ... |

## Shape Grammar
- [Rule that governs containers]
- [Rule that governs controls]
- [Rule that governs imagery or decoration]

## Type and Icon Grammar
- Type: [voice, hierarchy, contrast, line-length constraint]
- Icons: [stroke/fill, corner logic, optical weight, when labels are required]
```

## 3. Tokens and Components

```markdown
## Foundations
- Spacing: [base unit and rhythm]
- Radius: [small/medium/large roles]
- Borders and elevation: [when each is allowed]

## Component DNA
| Component | Role | Form | Color behavior | Interaction cue |
| --- | --- | --- | --- | --- |
| Primary action | ... | ... | ... | ... |
| Card/list item | ... | ... | ... | ... |
| Navigation | ... | ... | ... | ... |
| Input/selection | ... | ... | ... | ... |
```

Describe only components the product actually needs. Do not invent a component library.

## 4. Motion, Haptics, and States

```markdown
## Motion and Haptics
- Default character: [quiet/snappy/playful/etc.]
- Transition rule: [duration/easing range or relative rule]
- Haptics: [which irreversible or confirming moments deserve feedback]

## States
| State | Message hierarchy | Visual treatment | Action |
| --- | --- | --- | --- |
| Empty | ... | ... | ... |
| Loading | ... | ... | ... |
| Error | ... | ... | ... |
| Selected/pressed/disabled | ... | ... | ... |
```

State design is part of the visual system. Avoid decorative animation that delays a routine action.

## 5. Guardrails and Handoff

```markdown
## Do
- ...

## Don't
- ...

## Build Handoff
- Platform and accessibility constraints to respect
- Token naming and source of truth
- The first 2–3 screens/components to prototype
- Screenshot review criteria: hierarchy, color roles, shape consistency, state coverage
```

Finish with a compact implementation brief, not a generic list of design advice.

# Taste Profile, Risk, Platform, and Review Guide

Load only when preferences have become stable, when a direction needs a feasibility check, or when reviewing a rendered screen.

## Taste Profile

Keep this artifact compact enough to reuse in a future conversation:

```markdown
# [Product] Taste Profile
- Product and audience: ...
- North-star feeling: ...
- Visual anchors: ...
- Core tension: ...
- Color logic: ...
- Shape and density: ...
- Type and icon voice: ...
- Interaction character: ...
- Platform/accessibility constraints: ...
- Avoid: ...
```

Update only when the user makes a clear choice or supplies stronger visual evidence. Do not elevate a one-off reaction into a permanent preference. If a new choice conflicts with the profile, surface the conflict in one sentence and ask which choice should lead.

## Aesthetic Risk Check

Before recommending a direction or a major revision, test only the risks relevant to the product:

| Signal | Risk | Repair direction |
| --- | --- | --- |
| High-saturation palette + dense information | hierarchy and eye fatigue collapse | reserve saturation for actions and key status; quieten surfaces |
| Strong decorative language + serious/high-trust domain | tone feels careless or undermines credibility | move expression to moments, illustrations, and onboarding; keep task surfaces restrained |
| Fashion/editorial reference + long lists/forms | visual concept breaks under repetition | define list, form, and error-state variants before committing |
| Low-contrast material effect | weak legibility and poor state clarity | establish contrast floor and add non-color state cues |
| Trend-driven effect without product reason | rapid visual aging and generic identity | retain the underlying principle, remove the superficial effect |

Name a risk only when it applies to the supplied product. Pair every warning with a usable repair, never with a vague prohibition.

## Platform Translation

Treat Visual DNA as the invariant and platform patterns as the adaptation:

| Preserve across platforms | Adapt by platform |
| --- | --- |
| Color roles, type voice, shape grammar, icon character, motion temperament, content density | navigation convention, input behavior, system controls, safe areas, accessibility settings, haptic language |

For iOS, Android, or web, state the one or two native patterns that must remain familiar before applying the visual direction. Do not force identical components across platforms where interaction expectations differ.

## Screenshot Review Loop

Use this loop for a mockup, prototype, or implementation screenshot:

1. Load the Taste Profile and selected Visual DNA.
2. Check hierarchy, palette roles, shape/component consistency, type/icon voice, and visible states.
3. Identify the highest-leverage deviations only; three is the usual maximum.
4. Give each finding as `evidence -> consequence -> repair`.
5. Ask for the next most revealing screen: normally a list/detail pair, an input/selection state, or an empty/error state.

Use this compact output:

```markdown
## Visual DNA Review
**Aligned:** ...
**Repair first:**
1. [evidence] -> [consequence] -> [repair]
2. ...
**Review next:** [screen/state]
```

Do not score screens numerically unless the user explicitly wants a tracked audit. The point is to preserve coherence, not create a meaningless aesthetic grade.

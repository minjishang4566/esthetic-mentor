# Reference Sourcing Guide

Use sources for distinct jobs. Open only the one that can resolve the current design decision; a reference library is a map, not a required research phase.

## Source Hierarchy

| Layer | Resolve this question | Sources | Do not use it for |
| --- | --- | --- | --- |
| Visual ancestry | What lineage, formal vocabulary, or contrast does this direction belong to? | Style dictionaries and design-history references | Declaring an app usable or production-ready |
| Art and collections | What palette relationship, rhythm, material cue, or compositional tension is worth translating? | Museum collections and cultural archives | Treating an artwork as a UI template or a license to use its imagery |
| Furniture and product | How do form, proportion, construction, tactility, and ergonomics express the direction? | Design museums and furniture archives | Copying a recognisable object or treating a chair as an app layout |
| Contemporary evidence | Does the direction survive navigation, forms, lists, density, and states? | Current product/UI galleries and the user's own product | Establishing history or provenance |
| Colour and accessibility | Can the selected colour roles work as an accessible interface system? | Colour tools and contrast testing | Replacing judgement with an auto-generated palette |

### Token Rule

Do not browse this library before it changes a decision. When using one source, extract at most two transferable principles and return to the user with one relevant question or recommendation. Do not produce a source list unless the user asks for paths to explore.

## Visual Ancestry and Style Dictionaries

Use these when a user has a feeling, a partial reference, or conflicting influences but no reliable name for the visual language. Compare principles, not labels; an app may assign different roles to multiple lineages.

| Source | Use it for | Search by |
| --- | --- | --- |
| [IndexStyle](https://indexstyle.org/) | Sourced style names, provenance, intended effects, and explicit comparisons across historical, graphic, web, and app-interface languages | desired effect, medium, period, movement, or app context |
| [Design Style Book](https://www.designstylebook.com/) | Cross-disciplinary references across architecture, graphic design, typography, industrial design, interiors, and moving image | discipline, style name, material/form, or time period |
| [STYLEBASE](https://stylebase.art/) | A research-oriented visual-style archive for discovering and comparing visual vocabularies | style, movement, creator, or visual principle |

These references can help a mentor say, for example, "this is closer to quiet editorial structure than generic minimalism." They cannot justify piling several labels onto one product or replacing the user's own taste.

## Art and Cultural Collections

Use official collections when an app needs visual ancestry beyond current product references: colour-area relationships, framing, material, motif, visual tempo, and cultural context.

| Source | Use it for | Search by |
| --- | --- | --- |
| [Louvre Collections](https://collections.louvre.fr/) | Antiquity through the 19th century: painting, decorative arts, sculpture, textiles, objects, and furniture | period, region, material, object type, motif, or collection album |
| [The Met Open Access](https://www.metmuseum.org/pt/hubs/open-access) | Broad, well-documented public-domain works and object data; useful where a product needs both visual study and careful rights awareness | artist, culture, department, medium, object type, or period |
| [Rijksmuseum Collection](https://www.rijksmuseum.nl/en/collection) | Dutch art, decorative arts, still life, light, domestic atmosphere, and material detail | artist, material, object type, subject, or collection story |
| [Google Arts & Culture](https://artsandculture.google.com/) | A cross-institution discovery layer spanning artists, movements, media, themes, places, and collections | artist, movement, theme, medium, place, or colour/felt quality |
| [LACMA Collections](https://collections.lacma.org/) | Modern and contemporary art plus design traditions represented in Los Angeles | movement, artist, medium, region, collecting area, or visual principle |
| [MOCA Los Angeles](https://www.moca.org/) | Contemporary-art programming, artists, exhibitions, and collection context | artist, exhibition, medium, or theme |

For a selected work, extract no more than two transferable rules: a colour-area relationship, framing rhythm, contrast strategy, material cue, or shape tension. Do not treat the artist's name as a style prompt, reproduce a distinctive composition, or use artwork imagery without checking rights and obtaining the required permission.

## Furniture, Product, and Bauhaus References

Use these when the product needs a more grounded shape grammar than a screen gallery can supply. Study proportion, joins, weight, material contrast, repeat, and human use, then translate those principles into component geometry and interaction density.

| Source | Use it for | Search by |
| --- | --- | --- |
| [Vitra Design Museum Online Collection](https://collection.design-museum.de/en/) | Furniture, lighting, textiles, key designers, and manufacturer histories; especially useful for modernism and postwar design | designer, object type, material, collection, or era |
| [Bauhaus-Archiv Open Archive](https://open-archive.bauhaus.de/eMP/eMuseumPlus?module=collection&moduleFunction=search&service=ExternalInterface) | Primary Bauhaus objects, documents, furniture, textiles, photography, and workshop material | artist, object type, material, workshop, or date |
| [Cooper Hewitt Collection](https://collection.cooperhewitt.org/) | Product, textile, furniture, graphic, and interaction-design objects from a design-museum perspective | object type, material, maker, technique, or collection |
| [Designmuseum Danmark: Bauhaus](https://designmuseum.dk/en/exhibition/bauhaus/) | Bauhaus viewed through architecture, furniture, colour, movement, and its relationship to Danish design | Bauhaus, designer, furniture, colour, or movement |

Translate an object into a system rule, not a themed decoration. A tubular-steel chair may suggest an exposed linear structure and light visual weight; it does not imply putting chair silhouettes or Bauhaus primary colours into every screen.

## Contemporary Product Discovery

### Pinterest

[Pinterest](https://www.pinterest.com/) is optional and supplementary. Use it for fast visual discovery, adjacent references, user preference calibration, and a lightweight moodboard. It is not style authority, proof of provenance, or a source to copy from.

Build a query from two or three terms only:

`[style or visual principle] + [product/domain or medium] + [one constraint]`

Examples:

- `soft bauhaus mobile app warm cream`
- `swiss editorial finance dashboard color`
- `playful mid century habit tracker`

Prefer a visual principle when the user does not know a style name: `bold geometry`, `quiet editorial`, `friendly archival`, `soft tactile`, or `high contrast utility`.

After a search, invite the user to share anything that caught their attention or describe what they liked and disliked. Compare whatever evidence they provide before proposing a direction. Record repeated traits rather than individual pins.

### Product/UI Galleries

Use a current UI gallery only after a candidate direction exists and the question is practical: navigation, form density, onboarding, loading, empty states, accessibility, or responsive behaviour. The user's own app and screenshots are stronger evidence than a gallery. Do not use any gallery as a style authority or competitor-cloning source.

## Artist-Led Colour Discovery

Use this only when the user asks for colour inspiration or lacks a visual reference. Offer at most three paths chosen for the product's desired emotional temperature. Each path gives a search phrase, what to notice, and why it may fit; do not prescribe a fixed palette before the user selects a work.

| Colour path | Search phrase | What to notice | Useful when the product needs |
| --- | --- | --- | --- |
| Atmospheric blue and light | `Claude Monet Water Lilies blue violet` | layered cool hues, soft value shifts, and light held in a quiet field | calm, restorative, reflective presence |
| Singular blue intensity | `Yves Klein IKB blue works` | one saturated blue used as an immersive field, with space and material doing the supporting work | confident focus, cultural sharpness, a memorable accent |
| Relational colour study | `Josef Albers Interaction of Color` | how adjacent colours alter perceived brightness, warmth, and depth | precise systems where hierarchy matters more than decorative colour |
| Cut-paper contrast | `Henri Matisse cut-outs color composition` | high-chroma blocks, generous negative space, and clear colour-area balance | playful optimism, creative tools, or expressive onboarding |
| Colour-field stillness | `Mark Rothko color field paintings` | restrained palettes, soft edges, and emotional depth through value and scale | quiet premium, reflection, wellbeing, or focus experiences |

Do not describe a palette as a universal "Monet blue" or "Rothko red." A named artist is a discovery route, not a colour token. If the user shares a specific work or reaction, extract the visible relationships: dominant field, secondary field, contrast level, temperature, saturation, and accent placement. If they prefer to continue in words, use their description as provisional evidence.

## Colour Roles and Accessibility

Use colour tools after visual intent has been set. They verify and refine palette roles; they do not originate the product's taste.

| Source | Use it for | Constraint |
| --- | --- | --- |
| [Adobe Color](https://color.adobe.com/) | Extracting an initial relationship from an image, exploring harmonies, and recording candidate swatches | Reassign extracted colours to semantic roles and reduce them to a usable system; do not ship a five-swatch extraction as a UI palette |
| [APCA Contrast Calculator](https://apcacontrast.com/) | Checking text and icon contrast against actual background, size, and weight | Check the final foreground/background pairs in real component states, including disabled and dark mode where applicable |

Start with roles and proportions: dominant surface, raised surface, primary text, secondary text, accent/action, semantic states, and separators. Verify contrast only once those roles are placed in the actual interface.

## Reference Guardrails

- Search for a direction, never a competitor clone.
- Treat images as evidence of preference, not as instructions to reproduce.
- Check that selected references agree on at least two of: colour logic, composition, shape grammar, type voice, or emotional temperature.
- When references conflict, name the conflict and ask which side should lead. Example: "Do you prefer the calm whitespace of these images, or the saturated playful colour?"
- Favor a focused set of high-signal references, but never prescribe a quantity or require the user to supply images.
- Preserve cultural context. Do not reduce a movement, artwork, or craft tradition to a superficial surface treatment.

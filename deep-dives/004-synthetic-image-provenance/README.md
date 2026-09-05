# Deep dive 004 — Synthetic images, representation, and provenance

## Purpose

Replace vague claims about “AI images” with a concrete production map, then ask what appearance, metadata, and provenance can—and cannot—tell a viewer.

## Bounded question

What kind of object is a generated image, how did it come into being, and what evidence could warrant claims about its origin, transformations, depicted event, and responsible makers?

## Why reuse this

The framework can support future work on synthetic media, documentary trust, misinformation, model transparency, content credentials, and AI-assisted creative practice.

## Core references

- SRC-015 — [Rombach et al., “High-Resolution Image Synthesis with Latent Diffusion Models”](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html): technical mechanism for one influential architecture.
- SRC-016 — [C2PA specifications](https://spec.c2pa.org/specifications/): primary provenance framework; record the exact version read.
- SRC-012 — [Gunning on index and photographic truth claims](https://doi.org/10.1515/9780822391432-004).
- SRC-013 — [Rodowick on film's digital transition](https://www.jstor.org/stable/j.ctvjf9v4j).
- SRC-017 — [Zylinska on AI art](http://openhumanitiespress.org/books/download/Zylinska_2020_AI-Art.pdf).
- Pair with SRC-001 only after the technical production map is accurate.

## Technical reading rule

Do not attempt to become a machine-learning specialist in one day. Read SRC-015 to answer bounded questions: What is learned? In what space does generation occur? How does conditioning enter? What is sampled? What human selection happens outside the model? Do not generalize one architecture to all current systems.

## Production map

| Stage | Actors / systems | Inputs | Transformation or decision | Output | Evidence available |
|---|---|---|---|---|---|
| Dataset assembly | `[fill]` | `[fill]` | `[fill]` | training corpus | `[fill]` |
| Training | `[fill]` | corpus, objectives | `[fill]` | model weights | `[fill]` |
| Conditioning | `[fill]` | prompt / image / controls | `[fill]` | conditioning representation | `[fill]` |
| Generation | `[fill]` | noise, weights, condition | `[fill]` | candidate outputs | `[fill]` |
| Selection | `[fill]` | candidates | accept / reject / rerun | selected image | `[fill]` |
| Editing | `[fill]` | selected image | `[fill]` | finished asset | `[fill]` |
| Publication | `[fill]` | asset, caption, metadata | framing / disclosure | encountered work | `[fill]` |

## Trust matrix

| Question | Appearance can show | Provenance may show | Neither establishes by itself |
|---|---|---|---|
| Did the depicted event occur? | `[fill]` | `[fill]` | `[fill]` |
| Which tools were used? | `[fill]` | `[fill]` | `[fill]` |
| Who made meaningful choices? | `[fill]` | `[fill]` | `[fill]` |
| Is an assertion true? | `[fill]` | `[fill]` | `[fill]` |
| Is the work artistically successful? | `[fill]` | `[fill]` | `[fill]` |

## C2PA caution to preserve

The specification can make assertions and their association with an asset tamper-evident. Its own principles do not make value judgments about whether those assertions or the content are good, bad, or substantively true. Treat provenance as evidence infrastructure, not an oracle.

## Evidence placeholders

### DCLM-001 — Photographic appearance does not establish a photographed event

- **Technical support:** `[SRC and locator]`
- **Philosophical support:** `[SRC and locator]`
- **Counterexample or qualification:** `[fill]`
- **Status:** needs-research

### DCLM-002 — Provenance changes the trust question but does not settle it

- **Support:** `[SRC-016 version and section]`
- **Limitation:** `[fill]`
- **Normative inference:** `[fill]`
- **Status:** needs-research

## Done enough when

- One specific model and one specific output/work have complete production maps.
- You can explain generation in plain language without saying the model “imagines” or “knows” unless technically justified.
- You can distinguish provenance, authenticity, truth, and artistic value.
- Every claim about a current tool is dated and linked to primary documentation.

## AI prompt

“Audit this production map against the cited primary documentation. Identify missing human decisions, model steps I have anthropomorphized, and claims that apply only to this architecture. Do not infer undocumented training data or creative intention.”

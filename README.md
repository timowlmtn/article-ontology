# Ontology and AI Research Project

This repository is a source-first research and writing environment for a series about ontology and AI. It is designed to keep the writer responsible for thesis, judgment, conclusions, and final prose while making AI useful for discovery, organization, evidence tracing, critique, and verification.

The workflow borrows a useful principle from NotebookLM/Gemini Notebook: synthesis should be grounded in a bounded collection of sources selected by a human. Search results and generated text can help locate or interpret evidence, but they are not evidence themselves.

## Research pipeline

Every article moves through the same evidence gate. A stage can be revisited, but it should not be silently skipped.

1. **Frame** — complete the article brief and state a tentative, falsifiable thesis.
2. **Question** — turn uncertainties and likely objections into research questions.
3. **Discover** — log possible sources as `candidate`; search results are leads only.
4. **Accept** — the writer decides which sources enter the bounded article corpus.
5. **Read** — take attributed literature notes with page, section, or timestamp locators.
6. **Map evidence** — connect evidence to prospective claims, challenges, and gaps.
7. **Synthesize** — state what the evidence permits, disputes, or changes.
8. **Outline** — give every section an argumentative job and an evidence burden.
9. **Draft** — write in the writer's voice; keep observation distinct from sourced fact.
10. **Stress-test** — use AI as an adversarial reader and identify the strongest objection.
11. **Verify** — fact-check quotations, claims, links, dates, provenance, and fairness.

## Structure

- `ontology/`: provisional terms, concepts, and relationships
- `research/`: project questions, source catalog, research log, gaps, and inbox
- `sources/`: original or preserved source material, grouped by type
- `notes/`: attributed literature notes, concept notes, and synthesis
- `articles/`: bounded article workspaces and a reusable template
- `deep-dives/`: focused investigations that may support several articles
- `experiments/`: practical tests of ontology-centered research and AI architecture
- `archive/`: retired material retained for provenance

See `articles/README.md` for the article lifecycle and file contract. See `research/README.md` for source status and evidence provenance.

## Start a new article

Copy `articles/000-template/` to a numbered, descriptive directory. Complete `brief.md` first, then refine `questions.md`. Discover sources as candidates in the project catalog; only add accepted, article-relevant sources to the article's `sources.md`. Build `evidence.md` and `synthesis.md` before outlining or drafting.

## Working with AI

Use AI in named roles so its output remains inspectable:

- **Scout:** find candidate sources, originals, transcripts, and useful search paths.
- **Reader:** extract arguments and evidence with precise locators.
- **Cartographer:** compare definitions and map relationships among claims.
- **Adversary:** surface counterarguments, missing evidence, and category errors.
- **Interviewer:** question the writer after observation or field work without supplying answers.
- **Archivist:** maintain source IDs, statuses, provenance, and claim links.
- **Editor:** test structure and clarity only after the evidence is visible.
- **Fact-checker:** verify every externally checkable assertion against originals.

Ask AI to retrieve the smallest relevant context. Do not delegate final beliefs, source acceptance, thesis, fairness judgments, voice, or publication readiness to it. AI summaries and generated prose are not evidence.

## Useful prompts

- “Act as a source scout for AQ-___. Return candidates, not conclusions. Prefer primary sources.”
- “Read SRC-___. Separate quotation, source claim, interpretation, and open question.”
- “Map CLM-___ to supporting and challenging evidence. Do not strengthen the claim.”
- “Give the strongest informed objection to my thesis and specify what would answer it.”
- “Interview me about these field notes. Ask one concrete question at a time.”
- “Audit this draft against `evidence.md`; list unsupported or overstated claims.”

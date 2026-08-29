# Ontology and AI Research Project

This repository is a source-first research and writing environment for a series about ontology and AI. It is designed to keep the writer responsible for thesis, judgment, conclusions, and final prose while making AI useful for discovery, organization, evidence tracing, critique, and verification.

The workflow borrows a useful principle from NotebookLM/Gemini Notebook: synthesis should be grounded in a bounded collection of sources selected by a human. Search results and generated text can help locate or interpret evidence, but they are not evidence themselves.

## Research pipeline

1. Define and sharpen a question.
2. Plan the research, including competing views and counterarguments.
3. Discover candidate sources for writer review.
4. Accept or reject sources deliberately.
5. Take attributed notes from accepted sources.
6. Connect evidence to possible claims and record challenges and gaps.
7. Synthesize only after the evidence is visible.
8. Build an argumentative outline.
9. Draft in the writer's voice.
10. Fact-check claims, quotations, links, and source use.

## Structure

- `ontology/`: provisional terms, concepts, and relationships
- `research/`: project questions, source catalog, research log, gaps, and inbox
- `sources/`: original or preserved source material, grouped by type
- `notes/`: attributed literature notes, concept notes, and synthesis
- `articles/`: bounded article workspaces and a reusable template
- `deep-dives/`: focused investigations that may support several articles
- `experiments/`: practical tests of ontology-centered research and AI architecture
- `archive/`: retired material retained for provenance

## Start a new article

Copy `articles/000-template/` to a numbered, descriptive directory. Complete `brief.md` first, then refine `questions.md`. Discover sources as candidates in the project catalog; only add accepted, article-relevant sources to the article's `sources.md`. Build `evidence.md` before outlining or drafting.

## Working with AI

Use AI to expose choices, uncertainty, disagreement, unsupported claims, and promising research paths. Ask it to retrieve only the smallest relevant context. Do not delegate final beliefs, source acceptance, thesis, fairness judgments, or publication readiness to it. Generated prose belongs downstream of evidence and must never be cited as evidence.

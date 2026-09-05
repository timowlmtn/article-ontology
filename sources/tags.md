# Source tags

Tags make sources discoverable across articles and reference decks. They describe durable characteristics and uses; they do not replace catalog status, evidence evaluation, or prose descriptions.

## Syntax

Use lowercase namespaced tags in backticks:

- `topic/<subject>` — what the source concerns
- `form/<source-kind>` — what kind of source it is
- `role/<research-use>` — how it functions in an inquiry
- `access/<condition>` — how it can be retrieved or whether it changes
- `method/<approach>` — optional, for recurring research methods
- `place/<location>` — optional, for durable geographic or institutional retrieval

Use hyphens inside multiword tags: `topic/knowledge-representation`.

## Current topic tags

`topic/ai` · `topic/art` · `topic/auteur` · `topic/authenticity` · `topic/authorship` · `topic/criticism` · `topic/digital-media` · `topic/fieldwork` · `topic/film` · `topic/image-generation` · `topic/indexicality` · `topic/knowledge-representation` · `topic/law` · `topic/mediation` · `topic/medium` · `topic/museum` · `topic/ontology` · `topic/philosophy` · `topic/photography` · `topic/provenance` · `topic/realism` · `topic/representation` · `topic/technology`

This list should expand as the writer's workbench expands beyond ontology. Prefer ordinary subject language over building a theoretically perfect taxonomy.

## Current form tags

`form/article` · `form/book` · `form/chapter` · `form/essay` · `form/museum-record` · `form/paper` · `form/reference` · `form/report` · `form/standard` · `form/video`

## Current role tags

- `role/primary` — original text, research, standard, official record, or first-party account
- `role/secondary` — scholarly or critical interpretation
- `role/orientation` — useful entry point whose claims should lead to stronger sources
- `role/counterargument` — selected because it materially challenges a working thesis or dominant account
- `role/method` — reusable guidance for research or criticism
- `role/case-study` — concrete work, event, person, or implementation used to test a claim

A source can have more than one role when the roles are genuinely useful for retrieval.

## Current access tags

- `access/open` — openly accessible at the recorded link
- `access/library` — likely requires library or institutional access
- `access/paywalled` — publisher access requires payment or subscription
- `access/changing` — live page, standard, schedule, or other version-sensitive material
- `access/local` — lawful original preserved in this repository

## Article links

Tags answer “what is this useful for?” Article links answer “where is it currently being used?”

In `sources/index.md` and a local source-record README, link the article by its stable directory:

```markdown
[001-bazin-and-ai](../articles/001-bazin-and-ai/README.md)
```

Adjust `../` depth for the file's location. List multiple articles separately rather than inventing an article tag. Article links are relationships and should remain clickable.

## Adding a new tag

Add a tag when at least one condition holds:

- it retrieves two or more sources across the workbench;
- it marks a durable distinction needed by current research; or
- it is likely to organize a future reference deck.

Avoid tags for temporary status (`read-next`, `maybe`, `good`) or unsupported evaluation (`authoritative`, `true`). Put those judgments in the catalog, notes, or evidence records.

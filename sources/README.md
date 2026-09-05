# Sources — writer's workbench

Store original or preserved source material here after it has been deliberately accepted or when a local copy is needed for reliable access. Group it by source type: `primary/`, `academic/`, `industry/`, `books/`, or `web/`.

This is a general writing library, not an ontology-only collection. Sources may support any current or future article and can be regrouped into multiple reference decks without moving or duplicating the original material.

Do not edit an original source to incorporate interpretation. Put notes in `notes/literature/` and reference the stable source ID from `research/source-catalog.md`. Observe copyright and access restrictions; a catalog entry may point to an external source when retaining a local copy is inappropriate.

## Library index

Use `index.md` as the bridge between the project catalog and locally preserved material. It records all cataloged sources, including candidates that remain external-only.

Use `reference-decks.md` to find curated writer-facing research shelves. Individual decks live under `decks/` and group sources by the question they help answer. “Deck” here means a curated reference set, not a slide presentation.

The two files have different authority:

- `research/source-catalog.md` is the master record for identity, status, credibility, and use.
- `sources/index.md` records where or whether source material is preserved locally.
- `sources/reference-decks.md` indexes curated reading sets for particular articles or themes.
- `sources/tags.md` defines discoverable, reusable tags and article-link conventions.

Do not change a source from `candidate` to `accepted` merely because a local copy or source record exists.

## Local storage rules

- Preserve original bytes whenever a lawful downloadable original is retained.
- Do not rewrite, clean, or annotate original source files.
- Use filenames beginning with the stable source ID.
- Record download date, originating URL, edition/version, file type, and checksum in a neighboring README when useful.
- Store reading notes in `notes/literature/`, not beside or inside originals.
- For paywalled books and articles, retain only lawful copies supplied or obtained by the writer; otherwise keep the catalog link.
- For websites and changing standards, record an access date and version. Preserve a snapshot only when permitted and needed.
- For video, keep the stable video ID, channel, upload date, URL, caption provenance, and transcript verification status. Do not present automatic captions as an authoritative transcript.

## Categories

- `primary/` — original essays, research papers, standards, official reports, and first-party records
- `academic/` — scholarly interpretations, articles, and chapters
- `books/` — lawful local book or book-excerpt files; may overlap conceptually with primary or academic material
- `industry/` — vendor, consortium, or practitioner material requiring explicit source-context caution
- `web/` — online pages and audiovisual records, including SRC-020

Categories describe what a source is or where it is preserved. Tags describe what it can help you think about. One source can have many tags and support many articles without being copied into multiple category folders.

## Tags and article links

Every indexed source should have:

- at least one `topic/` tag;
- one `form/` tag;
- one `role/` tag;
- an `access/` tag when retrieval conditions matter; and
- direct links to every active article that currently uses or is evaluating it.

Use controlled tags from `tags.md` when possible. Add a new tag when it will help retrieve at least two sources or expresses a durable project distinction. Do not encode temporary reading status as a tag; status belongs in the catalog.

## Add an accepted source

1. Change its status in `research/source-catalog.md`, recording the decision reason.
2. Decide whether local preservation is lawful and useful.
3. Add the original file or a source-record README under the best-fit category.
4. Update `sources/index.md` with the relative path, version, and preservation status.
5. Create a literature note from `notes/literature/000-template.md`.
6. Link only the relevant accepted source from an article's `sources.md`.
7. Add or update its tags and article links in `sources/index.md`.

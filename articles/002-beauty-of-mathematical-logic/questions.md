# Article research questions — Beauty of mathematical logic

## Research table

| ID | Question | Why it matters | Evidence needed | Status | Next action |
|---|---|---|---|---|---|
| BMQ-001 | How does Malitz construct a first-order language and distinguish its symbols, terms, formulas, sentences, and derivations? | The article must begin with syntax before importing everyday ideas of truth. | Close reading of SRC-041's “The First Order Predicate Calculus,” with page locators. | open | Record one exact example and every new term in a glossary. |
| BMQ-002 | What is a structure, and how does it interpret a first-order language? | Establishes that strings of symbols do not bear the intended mathematical meaning on their own. | SRC-041's “Structures,” with page locators. | open | Make one language/structure interpretation table. |
| BMQ-003 | What does it mean for a structure to satisfy a formula or sentence, and when does a sentence count as true in a structure? | This is the article's first major bridge from formal syntax to semantic truth. | SRC-041's “Satisfaction and Truth,” with page locators and its own examples. | open | Record the exact relation and distinguish open formulas from sentences. |
| BMQ-004 | What is the relation—and nonidentity—between semantic consequence or validity and formal derivability? | Prevents “true,” “valid,” and “provable” from becoming interchangeable slogans. | SRC-041 plus an accepted supplement only if the selected pages leave a needed distinction open. | open | Identify whether Malitz states a soundness or completeness relation, and at what point. |
| BMQ-005 | Does the compactness theorem make the syntax/semantics relation vivid enough for a general reader? | It is the proposed complex theorem with an internal proof path. | SRC-041's compactness statement and proof; later explanatory source if accepted. | open | Read the theorem statement only after BMQ-001 through BMQ-004. |
| BMQ-006 | What does a proof assistant's kernel actually check, and what does it assume? | Prevents the false claim that AI itself validates a proof or that a check is assumption-free. | SRC-043 documentation, including trusted axioms, imported libraries, and proof terms. | open | Record accepted guarantees and stated limits in separate bullets. |
| BMQ-007 | How do contemporary AI systems interact with formal environments? | Distinguishes proposing/searching proof steps from checking them. | SRC-044 and SRC-045 methods, formalization requirements, evaluation, and limitations. | open | Build a contribution map: human formalizer, model, search procedure, library, kernel. |
| BMQ-008 | What does “beautiful” mean when mathematicians apply it to a proof? | Aesthetic language needs a source-grounded account, not the writer's intuition alone. | Primary or reflective writing by mathematicians; an explicit counterposition. | open | Discover candidates before selecting a definition. |
| BMQ-009 | Can semantic insight make an apparently mechanical derivation more intelligible without making formal validity secondary? | Tests the essay's central intuition without treating formalism as an enemy of understanding. | Malitz examples, a proof case, and a serious counterposition. | open | Write this first as a question in field notes, not a conclusion. |

## Candidate reading queue

All entries are `candidate` in `research/source-catalog.md`. The writer decides whether any enters `sources.md` as an accepted article source.

| Candidate | Question served | Priority | Why read it | Reading prompt | Decision |
|---|---|---:|---|---|---|
| SRC-041 — Malitz | BMQ-001–005 | 1 | Supplies the article's conceptual order and proposed theorem case. | How do syntax, structures, satisfaction, truth, and compactness build on one another? | unreviewed |
| SRC-043 — Lean reference | BMQ-006 | 1 | Makes the checking mechanism and its boundary precise. | What does the kernel check, and what does that not guarantee? | unreviewed |
| SRC-044 — LeanDojo | BMQ-007 | 2 | Documents an AI system's retrieval and proof-search workflow. | Which parts are learned search, environment feedback, and deterministic verification? | unreviewed |
| SRC-045 — AlphaProof | BMQ-007 | 2 | A current high-capability formal-reasoning case. | What was formalized, what did the agent search, and what did the environment verify? | unreviewed |

## Exit criteria before outlining

- The article has a source-grounded syntax/semantics map using Malitz's own terms.
- “Satisfaction,” “truth in a structure,” “formal derivability,” “checking,” and “understanding” each have source-grounded meanings.
- The roles of model, proof assistant, library, and human formalizer are visibly distinct.
- At least one account challenges the claim that beauty or explanation is required for mathematical value.
- The writer has decided whether compactness is the best eventual theorem case.

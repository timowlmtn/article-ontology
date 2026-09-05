# Article research questions

## Working inquiry

**Main question:** How, and under what conditions, could an ontology improve AI-assisted software development—and could those improvements reduce total model cost at Caylent without lowering quality?

**Writer's current hypothesis:** Explicitly modeled concepts and relationships may let an AI system retrieve a smaller, more relevant context, reducing input tokens and repeated explanation while improving consistency.

Treat that statement as a hypothesis. An ontology may add construction, maintenance, retrieval, and inference costs; a taxonomy, schema, curated documentation set, metadata filter, prompt cache, or conventional RAG system may deliver the same benefit more cheaply.

## Research table

| ID | Question | Why it matters | Status | Evidence needed / next step |
|---|---|---|---|---|
| AQ-001 | What does “ontology” mean in philosophy, knowledge representation, information science, and current AI engineering? | Prevents a cost-saving proposal from resting on an ambiguous word. It also exposes when two authors use the same term for different artifacts. | researching | Read SRC-C01 through SRC-C04. For each, record: definition, purpose, primitives, intended users, and what the author explicitly excludes. Build a one-page definition matrix; do not synthesize a single definition yet. |
| AQ-002 | What distinguishes an ontology from a taxonomy, controlled vocabulary, schema, knowledge graph, metadata model, embedding index, and document collection? | The hypothesis is only testable if the intervention is identifiable. Otherwise any structured retrieval system could be mislabeled “ontology.” | open | Make a comparison matrix with rows for each artifact and columns for hierarchy, typed relations, constraints/axioms, instances, inference, governance, and retrieval role. Ground disputed cells in SRC-C03, SRC-C05, SRC-C07, and SRC-C08. |
| AQ-003 | What would the ontology describe in an AI-assisted development system? | “Ontology for development” is too broad. The useful domain might be architecture, repositories, services, APIs, dependencies, requirements, decisions, incidents, teams, or some combination. | open | Interview 3–5 engineers. Collect ten expensive or repeatedly unsuccessful AI tasks. Identify the concepts and relationships needed to answer them. Write competency questions before modeling classes. |
| AQ-004 | Through what causal mechanism could an ontology reduce model usage or cost? | A graph does not save tokens by existing. Savings require a mechanism such as better routing, narrower retrieval, reusable identifiers, constraint checking outside the model, or less repeated explanation. | open | For each proposed mechanism, diagram: query → retrieval/planning → context assembly → model call → validation. State which tokens or calls disappear and which new costs appear. Seek counterexamples. |
| AQ-005 | Which baseline approaches could produce the same benefit without an ontology? | A fair test must compare against strong, simpler alternatives rather than an unstructured-document straw man. | open | Define baselines: curated docs, improved prompts, metadata filtering, conventional vector RAG, reranking, prompt caching, and a lightweight schema/taxonomy. Record operational effort for each. |
| AQ-006 | What does “cost” mean for Caylent, and what quality must be preserved? | API spend alone can fall while engineering time, latency, maintenance, or failure cost rises. A useful conclusion needs a total-cost boundary and quality floor. | open | Establish a baseline from representative tasks: input/output tokens, model calls, cached tokens, latency, dollar cost, success rate, groundedness, correction time, and ontology maintenance time. Redact client-sensitive data. |
| AQ-007 | What evidence exists that ontologies or knowledge graphs improve retrieval, reasoning, reliability, or context selection for LLM systems? | It separates plausible architecture from demonstrated outcomes and shows which findings transfer—or do not transfer—to software development. | open | Read SRC-C09 and SRC-C10 after the foundations. Extract task, dataset, baseline, metric, result, limitation, and whether the system actually uses a formal ontology rather than only a graph. |
| AQ-008 | What are the construction and lifecycle costs of an ontology? | Up-front modeling, extraction errors, schema drift, governance, and stale relations can overwhelm inference savings. | open | Read SRC-C05 and SRC-C06. Estimate initial and monthly effort for a narrow pilot. Identify owners, change triggers, validation rules, and a retirement condition. |
| AQ-009 | What is the smallest experiment that could falsify the cost-containment hypothesis? | A narrow, controlled test is more informative than building an enterprise ontology and attributing any later improvement to it. | open | Select one repeated, high-context development task. Freeze a question set and source corpus. Compare at least: vector RAG baseline, metadata/schema baseline, and ontology-assisted retrieval. Pre-register metrics and failure criteria. |
| AQ-010 | When would an ontology be the wrong intervention? | Boundary conditions protect against solutionism and make any positive recommendation more credible. | open | List rejection conditions: unstable domain, sparse reuse, low relationship value, cheap existing context, weak governance, high extraction error, or no measurable retrieval bottleneck. Ask interviewees for negative cases. |

Suggested statuses: `open`, `researching`, `answered provisionally`, `blocked`, `out of scope`.

## Candidate reading and listening

These are **candidates**, not accepted project sources. Review them before assigning permanent `SRC-###` IDs in `research/source-catalog.md`. The `SRC-C##` labels below are temporary reading-list handles.

### First pass: establish the meaning of ontology

| Candidate | Type | Priority | Why read it | Reading prompt |
|---|---|---:|---|---|
| SRC-C01 — Thomas Hofweber, [“Logic and Ontology,” Stanford Encyclopedia of Philosophy](https://plato.stanford.edu/entries/logic-ontology/) | Scholarly reference | Essential | Separates several philosophical projects carried under “ontology” and prevents importing the computational sense backward into philosophy. | What questions does philosophical ontology ask that an engineering ontology does not? |
| SRC-C02 — Thomas R. Gruber, [“A Translation Approach to Portable Ontology Specifications”](https://tomgruber.org/writing/ontolingua-kaj-1993.pdf), *Knowledge Acquisition* 5(2), 1993 | Foundational paper | Essential | A primary source for the influential knowledge-engineering account of ontology and its original goals of knowledge sharing and reuse. | What is being made portable, for whom, and by what representational commitments? |
| SRC-C03 — Nicola Guarino, Daniel Oberle, and Steffen Staab, [“What Is an Ontology?”](https://iaoa.org/isc2012/docs/Guarino2009_What_is_an_Ontology.pdf), in *Handbook on Ontologies*, 2009 | Foundational chapter | Essential | Directly compares philosophical and computational senses and refines the language of conceptualization and specification. | Which distinctions clarify Gruber, and which introduce additional commitments? |
| SRC-C04 — Katherine Munn and Barry Smith, eds., [*Applied Ontology: An Introduction*](https://doi.org/10.1515/9783110324860), 2008 | Book | Recommended | Shows how philosophical category analysis becomes applied modeling, especially in scientific and biomedical information systems. | Which realist assumptions are useful, optional, or contentious for software-development knowledge? |

**Deliverable after this pass:** a definition matrix with no “winner.” Include at least philosophical ontology, formal ontology, domain ontology, application ontology, and ontology artifact.

### Second pass: learn how ontologies are engineered

| Candidate | Type | Priority | Why read it | Reading prompt |
|---|---|---:|---|---|
| SRC-C05 — Natalya F. Noy and Deborah L. McGuinness, [“Ontology Development 101”](https://protege.stanford.edu/publications/ontology_development/ontology101-noy-mcguinness.html), Stanford, 2001 | Practical guide | Essential | A compact, influential guide to scope, reuse, classes, properties, instances, and iterative evaluation. | Translate its domain-and-scope questions into competency questions for one Caylent use case. |
| SRC-C06 — Mike Uschold and Michael Grüninger, [“Ontologies: Principles, Methods and Applications”](https://doi.org/10.1017/S0269888900007797), *Knowledge Engineering Review* 11(2), 1996 | Survey/method paper | Essential | Connects motivations, degrees of formality, development methods, and application patterns. | Which claimed benefits are mechanisms, and which are outcomes that still require evidence? |
| SRC-C07 — Steffen Staab and Rudi Studer, eds., [*Handbook on Ontologies*, 2nd ed.](https://link.springer.com/book/10.1007/978-3-540-92673-3), 2009 | Reference book | Selective | Broad reference on representation languages, engineering, reasoning, infrastructure, and applications. | Read selectively: the opening definition chapter plus chapters relevant to the pilot; do not read cover to cover initially. |
| SRC-C08 — Aidan Hogan et al., [“Knowledge Graphs”](https://doi.org/10.1145/3447772), *ACM Computing Surveys* 54(4), 2021 | Survey paper | Essential | Maps graph data models, schemas, identity, context, quality, and knowledge-graph terminology—the nearest neighboring field. | Mark every place where “knowledge graph” does and does not entail an ontology. |
| SRC-C11 — Pascal Hitzler et al., eds., [*Ontology Engineering with Ontology Design Patterns*](https://www.sagepub.com/shop/buy-a-book/ontology-engineering-with-ontology-design-patterns-foundations-and-applications-1-297384), 2016 | Book | Later | Introduces reusable modeling patterns and modular construction after the basic distinctions are secure. | Which patterns could support a small, evolvable pilot rather than an enterprise-wide model? |

**Deliverable after this pass:** a comparison table for ontology, taxonomy, schema, and knowledge graph, followed by 8–12 competency questions for one development workflow.

### Third pass: connect the foundations to LLM systems

| Candidate | Type | Priority | Why read it | Reading prompt |
|---|---|---:|---|---|
| SRC-C09 — Shirui Pan et al., [“Unifying Large Language Models and Knowledge Graphs: A Roadmap”](https://doi.org/10.1109/TKDE.2024.3352100), *IEEE TKDE* 36(7), 2024 | Survey paper | Essential after foundations | Organizes KG-enhanced LLMs, LLM-augmented KGs, and systems where both interact. Useful as a map, not proof of cost savings. | Which categories could narrow context or replace model work, and where are costs merely shifted? |
| SRC-C10 — Darren Edge et al., [“From Local to Global: A Graph RAG Approach to Query-Focused Summarization”](https://arxiv.org/abs/2404.16130), 2024 | System paper | Recommended | Provides a concrete graph-based retrieval architecture and evaluation to critique. Its generated entity graph is not automatically equivalent to a governed formal ontology. | Compare indexing cost, query cost, context size, task type, and quality against its baselines. |
| SRC-C12 — W3C, [*OWL 2 Web Ontology Language: Document Overview*, 2nd ed.](https://www.w3.org/TR/owl2-overview/), 2012 | Standard overview | Later/reference | Shows what a formal web ontology language can express and what reasoning commitments “ontology” may imply technically. | Which expressive features would the pilot truly use? What can remain lightweight? |

**Deliverable after this pass:** a mechanism map connecting ontology features to measurable system effects. Do not record “knowledge graphs help LLMs” as a single undifferentiated claim.

### Podcasts and talks: orientation and practitioner counterpoints

Podcasts are secondary sources. Use them to learn vocabulary, discover examples, and identify claims to verify—not as decisive evidence.

| Candidate | Type | Priority | Why listen/watch | Verification task |
|---|---|---:|---|---|
| SRC-C13 — *Talk Tech with Data Dave*, [“Ontology vs. Taxonomy: How AI Uses Knowledge Graphs”](https://d3clarity.com/podcast/ontology-vs-taxonomy-ai-knowledge-graphs/), with Erik Lee, 2025 | Podcast | Optional orientation | A short practitioner explanation of the ontology/taxonomy/knowledge-graph distinction. | List every definitional claim and test it against SRC-C03 and SRC-C08. |
| SRC-C14 — *Earley AI Podcast*, [“Taxonomy, Knowledge Graphs, and the Excuse Case”](https://www.earley.com/insights/earley-ai-podcast-episode-13-stephanie-lemieux-dovecot-studio), with Stephanie Lemieux, 2022 | Podcast | Recommended practitioner view | Emphasizes use-case discipline, content operations, and the risk of adopting graphs without a defined problem. | Extract one positive and one negative adoption criterion for the Caylent pilot. |
| SRC-C15 — *Earley AI Podcast*, [“Why AI Is a Content Problem”](https://www.earley.com/insights/earley-ai-podcast-episode-23-andy-fitzgerald), with Andy Fitzgerald, 2022 | Podcast | Optional | Connects content models, Schema.org, boutique ontologies, and knowledge graphs in an enterprise setting. | Separate claims about content quality from claims unique to ontology. |
| SRC-C16 — Jesús Barrasa, [*Going Meta: Using Ontologies to Guide Knowledge Graph Creation from Unstructured Data*](https://neo4j.com/videos/going-meta-s02-ep-01-continuing-the-journey-in-ai-and-knowledge-graph/), Neo4j | Technical talk/demo | Later | Demonstrates schema/ontology choices, extraction, constraints, and graph construction with contemporary tools. It is vendor-produced and should be read accordingly. | Identify which steps require model calls, human governance, and ongoing maintenance. |

## Recommended sequence for the next four working sessions

1. **Vocabulary session (90 minutes):** Read SRC-C01 selectively, then SRC-C02 and SRC-C03. Fill the definition matrix. Record disagreements rather than resolving them.
2. **Boundary session (90 minutes):** Read SRC-C05 and the relevant sections of SRC-C08. Build the neighboring-artifacts comparison matrix.
3. **Caylent problem session (60–90 minutes):** Gather ten costly development prompts or workflows. Cluster them by failure mode: excessive context, repeated background, poor retrieval, hallucination, tool misuse, or rework. Do not assume ontology addresses every cluster.
4. **Pilot-design session (90 minutes):** Write competency questions, choose one narrow workflow, define baselines and metrics, and state a result that would cause you to reject the ontology approach.

## Evidence worksheet for every source

For each accepted source, capture:

- **Source says:** a paraphrase with page/section locator
- **Exact quotation:** only when wording matters, with locator
- **Source's purpose and context:** what problem it is addressing
- **Definition of ontology:** or note that none is supplied
- **Claim relevant to Caylent:** kept narrower than the source's claim
- **Challenge or limitation:** including competing definitions
- **Your interpretation:** clearly labeled
- **Question opened:** what must be researched next

## Exit criteria for this foundational step

Do not move to implementation until you can:

- explain at least three materially different senses of “ontology”;
- distinguish an ontology from a taxonomy, schema, knowledge graph, and embedding index without relying on slogans;
- name the exact development domain and users for a pilot;
- write 8–12 competency questions the pilot must answer;
- identify the causal path by which the ontology might reduce model calls or tokens;
- define strong non-ontology baselines and total-cost metrics; and
- state conditions under which you would conclude that ontology is unnecessary overhead.

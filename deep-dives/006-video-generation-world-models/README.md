# Deep dive — Video generation, world models, and cinematic realism

## Purpose

Build a reusable, technically grounded account of the difference between generating plausible moving images and learning a causal representation that can predict the consequences of actions.

## Bounded question

What does Yann LeCun mean when he argues that pixel-level video prediction is inadequate for world understanding, and how well do current video-generation systems answer that criticism?

## Why reuse this

This distinction can support articles about AI cinema, simulation, robotics, visual evidence, narrative continuity, games, and synthetic media. It should prevent three recurring errors:

- treating a visually convincing clip as proof that a model understands physics;
- treating physical accuracy as sufficient for cinematic realism; and
- treating LeCun's non-generative V-JEPA work as a movie-generation system.

## Provisional answer

LeCun's target is not video-making as such. His claim is that a system trained to reconstruct or predict every visual detail must represent a vast, uncertain distribution of possible future pixels. For understanding, prediction, and planning, he argues that the model should instead discard unpredictable detail and predict in an abstract representation space. V-JEPA and V-JEPA 2 operationalize that proposal, but they do not render finished movies.

The competing view, stated by OpenAI in the Sora reports, is that scaled generative video models can acquire useful simulation capabilities. The first Sora report also documented failures in basic interactions, object-state changes, long-duration coherence, and spontaneous object appearance. Newer systems claim meaningful improvements. Independent 2025 benchmarks nevertheless found substantial remaining deficits in physical commonsense, especially in demanding actions and conservation laws.

## Core references

- SRC-021 — LeCun, *A Path Towards Autonomous Machine Intelligence*: architectural thesis for predictive world models and JEPA.
- SRC-022 — Bardes et al., “Revisiting Feature Prediction…”: V-JEPA predicts masked video regions in representation space.
- SRC-023 — Assran et al., “V-JEPA 2”: current evidence for video-learned understanding, prediction, and robot planning.
- SRC-024 — LeCun and Manyika, “Learning Abstractions”: LeCun's clearest recent explanation of why future-pixel prediction is intractable.
- SRC-025 — Big Technology interview with LeCun: direct audiovisual example of generated-video physics failures; transcript requires audio verification.
- SRC-026 — OpenAI, “Video generation models as world simulators”: explicit competing hypothesis and documented Sora limitations.
- SRC-027 — Bansal et al., VideoPhy-2: human-evaluated physical-commonsense benchmark.
- SRC-028 — Meng et al., PhyGenBench: peer-reviewed benchmark across 27 physical laws.
- SRC-029 — Google DeepMind, Veo 3.1: current first-party capability claims and short-clip production context.
- SRC-030 — OpenAI, “Sora 2 is here”: later first-party improvement claims and product-status record.
- SRC-031 — Bazin, *What Is Cinema?*, volume 2: primary critical basis for the *Bicycle Thieves* comparison.

All remain candidates until the writer reviews them.

## A three-session study path

### Session 1 — Understand LeCun's objection

1. Read SRC-024, pp. 46–51, marking every distinction among pixels, representations, prediction, generation, causality, and planning.
2. Read the abstract and architecture sections of SRC-021.
3. Write a two-column note: “details needed to render a shot” versus “state needed to predict an outcome.”

### Session 2 — See what JEPA actually demonstrates

1. Read SRC-022's abstract, method overview, and limitations.
2. Read SRC-023's abstract, evaluation design, and robot-planning sections.
3. Record what the systems demonstrate and what they do not: recognizing motion, anticipating action, and planning are not equivalent to generating a coherent film.

### Session 3 — Test the competing generative claim

1. Read SRC-026's method and discussion, especially its self-reported failures.
2. Read SRC-027 and SRC-028 for independent tests of physical commonsense.
3. Inspect SRC-029 and SRC-030 as first-party evidence of later progress, keeping vendor claims separate from independent evaluation.
4. Decide whether the article needs a controlled clip experiment: the same mundane action generated several times, evaluated for object persistence, consequence, and ordinary contingency.

## Bicycle Thieves bridge

Use the comparison as a question, not yet as a conclusion:

> Can a model generate a succession of plausible images while failing to sustain the ordinary causal world that makes *Bicycle Thieves* believable?

Bazin's account of the film is not a physics benchmark. Its realism involves contingency, social situation, ambiguity, duration, performance, framing, and the spectator's freedom—not merely correct gravity or object permanence. The technical evidence can establish a gap between surface plausibility and stable causal continuity. It cannot by itself establish whether a generated film has truth, moral force, authorship, or artistic value.

## Museum exercise

While walking the museum, choose three works that imply time or consequence: an action about to occur, a material under force, or a before-and-after relation. For each, note:

1. What visual detail makes the represented world feel stable?
2. What causal sequence do you supply rather than see?
3. What depends on physical plausibility, and what depends on convention or interpretation?
4. Would a technically perfect simulation settle what the work means?

Bring those notes back to this deep dive before applying them to AI cinema.

## Done enough when

- LeCun's claim can be stated without saying that he proved generative video can never work.
- V-JEPA is clearly distinguished from a video generator.
- At least one independent benchmark and one current system report have been read closely.
- The Bazin connection names both its genuine insight and its categorical limit.
- Any quotation from the interview has been checked against the audio.

## AI prompt

“Act as a skeptical technical reader. Using only the source passages and locators I provide, separate claims about visual generation, physical prediction, causal world models, planning, and cinematic realism. Identify where I infer understanding from appearance or artistic value from physical consistency. Do not write article prose.”

## Files

- `brief.md` — boundary and completion condition
- `questions.md` — open questions and next actions
- `sources.md` — accepted deep-dive corpus; empty until writer acceptance
- `evidence.md` — prospective claims, support, and challenges
- `synthesis.md` — reusable conclusions after reading

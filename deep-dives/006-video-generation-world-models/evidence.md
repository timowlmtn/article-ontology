# Evidence — Video generation and world models

These are prospective claims. Source discovery is complete enough to begin reading, but the writer has not accepted the sources and most quotations still require full-text or audio verification.

## VCLM-001 — LeCun distinguishes rendering from understanding

- **PROSPECTIVE CLAIM:** LeCun does not argue that generative systems cannot make videos. He argues that predicting every future pixel is an inefficient and possibly intractable route to the abstract state representations required for prediction and planning.
- **SOURCE CLAIM:** SRC-024 says future video frames contain too many unspecified details for a useful pixel-level distribution and argues for prediction in an abstract representation space.
- **LOCATOR:** SRC-024, pp. 47–51, especially pp. 48–49 and 51.
- **SUPPORT:** SRC-021 supplies the broader architecture; SRC-022 implements feature prediction from video.
- **CHALLENGE:** SRC-026 and SRC-030 explicitly argue that scaled generative video can develop simulation abilities.
- **SCOPE:** This is a dispute about learning objectives and usable world models, not a proof about the aesthetic limits of generated cinema.
- **STATUS:** needs-reading

## VCLM-002 — V-JEPA is non-generative

- **PROSPECTIVE CLAIM:** V-JEPA learns from video by predicting masked regions in representation space rather than reconstructing the pixels, so its success cannot be shown as an example of an AI-generated movie.
- **SOURCE CLAIM:** SRC-022 reports feature-prediction results for motion and appearance tasks; SRC-023 extends the program to action anticipation and robot planning.
- **SUPPORT:** SRC-022 abstract and method; SRC-023 abstract and robot-planning evaluation.
- **CHALLENGE:** “Non-generative” describes the training/output objective at issue; downstream systems could potentially combine a learned representation with a renderer.
- **STATUS:** needs-reading

## VCLM-003 — Current generators remain strongest at bounded clips

- **PROSPECTIVE CLAIM:** Current systems can produce striking short clips with improving control, sound, and apparent physical behavior, but this is not yet equivalent to autonomous feature-film generation with stable characters, objects, spaces, causes, and consequences.
- **SUPPORT:** SRC-029 reports Veo 3.1 comparisons on clips of roughly 6–10 seconds and offers scene extension and reference controls. SRC-030 reports multi-shot and state-persistence improvements in Sora 2 while also calling the model imperfect.
- **CHALLENGE:** Production workflows can assemble many generated shots under human direction; “cannot make a movie” is too absolute unless “movie” and the required autonomy are defined.
- **SCOPE:** Distinguish one-shot generation, edited sequences, and end-to-end long-form generation.
- **STATUS:** needs-independent-evidence

## VCLM-004 — Physical commonsense is still an empirical weakness

- **FACT CLAIM:** In VideoPhy-2's human evaluation, the best evaluated model reached 22% joint semantic-and-physical adherence on the hard subset; conservation of mass and momentum were particular difficulties.
- **SUPPORT:** SRC-027, abstract/results summary.
- **SOURCE CLAIM:** PhyGenBench reports that evaluated models struggle with physical commonsense and that scaling or prompt engineering alone did not solve its dynamic scenarios.
- **SUPPORT:** SRC-028, abstract and results.
- **CHALLENGES:** Benchmarks test chosen prompts and model versions, not every current system or cinematic genre. Evaluators may conflate familiar appearance with correct mechanics, while intentionally impossible cinema should fail a literal physics test.
- **STATUS:** needs-method-reading

## VCLM-005 — The strongest Bazin bridge is causal continuity, not photorealism

- **AI INFERENCE:** A generated clip can resemble location-shot cinema while lacking stable causal consequences across time. This makes LeCun useful for distinguishing appearance from a represented world's continuity.
- **BAZINIAN SUPPORT NEEDED:** SRC-031, “Bicycle Thief” and “De Sica: Metteur en scène,” on events retaining their weight, singularity, and ambiguity; and on artifice becoming unobtrusive rather than absent.
- **TECHNICAL SUPPORT:** SRC-024, SRC-026, SRC-027, SRC-028.
- **CHALLENGE:** Bazinian realism is not reducible to physical accuracy. The film's social relations, contingency, performance, framing, duration, and spectator activity exceed a world-model benchmark.
- **STATUS:** hypothesis

## VCLM-006 — “Optimize the most dramatic shot” may invert Bazin

- **WRITER IDEA UNDER TEST:** Could an AI recreate *Bicycle Thieves* by calculating the most dramatic angle, event, and outcome?
- **AI INFERENCE:** Bazin's praise may point in the opposite direction: De Sica's aesthetic labor makes events seem sufficient in themselves, without conspicuous directorial emphasis. An optimizer trained toward conventional dramatic salience could erase the incidental delays and ambiguities Bazin values.
- **SUPPORT NEEDED:** Full Bazin essay; a documented objective or preference model used in video generation; a controlled scene experiment.
- **CHALLENGE:** Human filmmakers also select, rehearse, frame, and edit. “Invisible” form is not absence of authorship or optimization.
- **STATUS:** promising-question

## Interview transcript record

- **Video:** SRC-025, Big Technology Podcast, 19 March 2025.
- **Relevant chapters:** 37:24, “Why video generation systems don't equal real comprehension”; broader world-model discussion begins around 29:37.
- **Third-party transcript:** Podscripts provides a searchable transcript, including the generated-wine example around 37:22–37:56 and the abstraction example around 41:50.
- **Verification status:** usable for navigation, not yet authoritative for quotation. Check the wording against the YouTube audio and determine whether YouTube captions are creator-provided or automatic.

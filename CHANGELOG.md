# Changelog

This file records the development history of the ATHENA framework. It describes **what** was introduced and **when**, not how it is implemented.

Dates refer to the author's internal working versions. The public repository is updated at milestones.

---

## [2026.2] — November 2026

Public update reflecting the move from conceptual framework to operational analytical chain.

### Added

- **Archetypal reading** (upstream identification layer). Identification of the emitter's archetypal figure and state (light / shadow), the roles assigned to other actors, the observed or anticipated slide between states, and the implicit target the message is designed for. Identified once per case, under evidence, and shared with the poles as a descriptive fact.
- **Reactance module.** Psychological reactance assessed as a dedicated module, separating factors carried by the message from factors carried by the audience's social and historical context. BOUCLIER is derived from it.
- **Reception substrate.** Structured description of the terrain prior to the message (institutional distrust, polarization, social demand for narratives), so that the analysis is not centred on the supply side only.
- **Objective-setting stage.** Explicit step between upstream material and pole assessment: immediate narrative objective and long-term strategic aim are fixed before any scoring, to avoid circularity.
- **Disambiguation of "it works".** Three distinct output variables: altering a perception, installing a belief, triggering a behaviour. The relevant one is fixed upstream.
- **Interoperability with DISARM and [DIMA](https://github.com/M82-project/DIMA) (M82 project).** Attacker-side descriptions are ingested as upstream material, kept on their own plane and never aggregated into the audience-side assessment.
- **Temporal layer.** Narrative half-life, narrative phase, and case mode (one-shot vs cumulative campaign) as a relevance precondition.
- **Declared veracity.** Each case carries a veracity status declared by the analyst (true / false / malinformation / not declared). ATHENA never produces this status itself. The same resistance level reads differently depending on it: healthy resistance to a falsehood, or rejection of a true message.
- **Epistemic doctrine.** Evidence contract on inputs (factual / deduced / not assessable) and four proof regimes on outputs (see `docs/epistemic-doctrine.md`).
- **LLM-assisted, human-in-the-loop chain.** Language models produce structured proposals under an evidence contract; the analyst arbitrates, completes context-dependent assessments, and validates. Single-revision rule on contested assessments.
- **Two-level output.** Analyst report and jargon-free decision-maker briefing.
- **Retrospective case:** Doppelganger, "bedbugs" wave, France, October 2023.

### Changed

- Theoretical anchor made explicit: psychological reactance (Brehm, 1966; Dillard & Shen, 2005), not the "backfire effect" (Nyhan & Reifler, 2010; see Wood & Porter, 2019).
- French version of the public documentation (`fr/`).
- Repositioning: ATHENA ranks **reception hypotheses**; it does not predict behaviour.
- Back-testing concordance redefined accordingly: agreement on the hierarchy of retained hypotheses, not on a behavioural threshold.

### Development milestones (internal)

| Period | Milestone |
|---|---|
| June 2026 | Temporal and strategic layer framed; objective-setting stage defined |
| July 2026 | Reactance module consolidated; output observability triage (four proof regimes); declared-veracity field; reception substrate |
| October 2026 | Archetypal reading formalised as an upstream layer; LLM proposal contract and analyst input tool; first full retrospective case processed end to end |

---

## [2026.1] — 9 March 2026

First public release.

- Four-pole conceptual framework: CORPS, TERRAIN, BOUCLIER, VECTEUR
- Influence / resistance diagnostic matrix
- Basic analytical workflow
- Illustrative case: COVID-19 / 5G narrative

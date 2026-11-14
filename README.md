# ATHENA Framework
### A Reception-Analysis Framework for Narrative Influence

*Version française : [`fr/README.md`](fr/README.md)*

ATHENA is an analytical framework for studying **how narratives are received**: why a message is absorbed, amplified, ignored, or rejected by a given audience, in a given context, at a given moment.

Rather than treating narratives as isolated persuasive contents, ATHENA interprets them as **perturbations within a collective cognitive system**. Depending on the configuration of that system, the same narrative may take hold, stagnate, or trigger an opposing reaction.

![License](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey)
![Status](https://img.shields.io/badge/status-operational%20research%20framework-blue)
![Domain](https://img.shields.io/badge/domain-narrative%20reception-orange)
![Version](https://img.shields.io/badge/public%20version-2026.2-green)

---

## What ATHENA Does

ATHENA structures reception analysis around **four interacting analytical poles**.

| Pole | What it observes |
|---|---|
| **CORPS** | Narrative structure of the message |
| **TERRAIN** | Psychological, cultural and social configuration of the audience |
| **BOUCLIER** | Defensive mechanisms and psychological reactance |
| **VECTEUR** | Activation and propagation dynamics |

Together these poles help analysts understand not only whether a narrative is strong, but **why it works, fails, stalls, polarizes, or triggers reactance** for a specific audience.

Since its first public release (March 2026), ATHENA has moved from a conceptual model to an **operational analytical chain**, tested on retrospective cases of foreign information manipulation.

---

## Core Insight

ATHENA shifts narrative analysis from **content analysis** to **reception analysis**.

It helps answer questions such as:

- Why does a seemingly strong narrative fail?
- Why does a mediocre narrative go viral?
- When does narrative pressure produce reactance instead of persuasion?
- When is a public denunciation likely to amplify the very narrative it targets?
- Which part of a diagnosis can be checked against observable reality, and which part remains a hypothesis?

---

## What Is New in 2026.2

The four-pole core is unchanged. Around it, ATHENA now includes:

| Component | Role |
|---|---|
| **Archetypal reading** | An upstream identification layer: which figure the emitter embodies, which roles it assigns to others, and towards which "shadow" or "light" state the narrative is sliding. Identified once, under evidence, then shared with the poles. |
| **Reactance module** | BOUCLIER is now assessed through a dedicated module that separates reactance carried by the message itself from reactance carried by the audience's social context. |
| **Reception substrate** | A structured description of the terrain *before* the message arrives: institutional distrust, polarization, social demand for certain narratives. |
| **Objective-setting stage** | Before any assessment, the analyst fixes what the narrative is trying to achieve (alter a perception, install a belief, trigger a behaviour) and its long-term strategic aim. Poles assess against that objective, not in the abstract. |
| **Interoperability with DISARM and DIMA** | Attacker-side descriptions (tactics, cognitive techniques) are ingested as upstream material. They inform the reception analysis without being merged into it. |
| **Temporal layer** | Narrative half-life, narrative phase, and the distinction between one-shot operations and cumulative campaigns. |
| **Epistemic doctrine** | Every input carries its evidential status; every output carries its proof regime. ATHENA states what can be verified, and what cannot. |
| **Human-in-the-loop, LLM-assisted chain** | Language models propose structured assessments under an explicit evidence contract; the analyst arbitrates, completes the context-dependent parts, and validates. |
| **Two-level output** | An analyst report, and a jargon-free briefing for decision-makers. |

See `CHANGELOG.md` for the dated history of these developments.

---

## System Architecture

```text
             UPSTREAM MATERIAL
   Archetypal reading · Attacker-side frameworks
   (DISARM, DIMA) · Reception substrate
                    │
                    ▼
            OBJECTIVE SETTING
   Immediate narrative objective · Long-term aim
                    │
                    ▼
                VECTEUR
          (Activation / diffusion)
                    ▲
                    │
CORPS ◄──────── System configuration ───────► TERRAIN
(Narrative structure)              (Audience configuration)
                    │
                    ▼
               BOUCLIER
       (Reactance / defensive threshold)
                    │
                    ▼
     ANALYST VALIDATION → DIAGNOSIS → BRIEFING
                    │
                    ▼
          Observable checks (RETEX)
```

## Core Principle

Narrative impact emerges from the **interaction between influence forces and resistance forces**.

| Influence | Resistance | Outcome |
|-----------|------------|--------|
| High | Low | Narrative adoption |
| High | High | Conflict / polarization |
| Low | Low | Information inertia |
| Low | High | Defensive rejection |

### Configurations this reveals

**False strong messages.** A narrative looks persuasive but fails because it triggers strong defensive reactions.

**Weak messages that go viral.** A mediocre narrative spreads because the whole system is aligned: receptive terrain, low resistance, strong vector.

**Narrative tipping points.** Increasing pressure on a resistant audience worsens the situation: source derogation, hardening of the threatened position, counter-mobilization.

**Weak attack on fragile terrain.** The danger lies less in the message than in the state of the audience it lands on. Over-reacting can do more harm than the operation itself (see `cases/doppelganger-bedbugs-2023.md`).

---

## Analytical Workflow (summary)

1. Gather upstream material (archetypal reading, attacker-side description, reception substrate)
2. Fix the objective of the narrative
3. Assess the four poles, each blind to the others' scores
4. Complete and validate the context-dependent assessments (analyst)
5. Diagnose the configuration and check it against the analyst's reading
6. Produce the analyst report and the decision-maker briefing
7. State the observables that would confirm or refute the diagnosis

Detailed documentation:

- `docs/conceptual-foundations.md`
- `docs/system-architecture.md`
- `docs/analytical-workflow.md`
- `docs/epistemic-doctrine.md`
- `docs/limitations-and-scope.md`
- `docs/references.md`

Cases:

- `cases/covid-5g-narrative.md`: illustrative conceptual case
- `cases/doppelganger-bedbugs-2023.md`: retrospective case, analysed with the operational chain

---

## Applications

- foreign information manipulation and interference (FIMI) analysis
- counter-narrative design reasoning
- red teaming of strategic or crisis communication
- anticipation of reception risk before publication
- research on misinformation and reactance

## Positioning

ATHENA is designed as **complementary** to attacker-side frameworks.

- **[DISARM](https://github.com/disarmfoundation)** describes what happened in an influence campaign (tactics, sequence, actors).
- **[DIMA](https://github.com/M82-project/DIMA)**, developed by the M82 project, describes which cognitive techniques a manipulation relies on.
- **ATHENA** analyses **how the targeted audience is likely to receive it**, and why.

## Theoretical Anchor: Reactance, Not the "Backfire Effect"

ATHENA's resistance pole is grounded in **psychological reactance theory** (Brehm, 1966) and the intertwined model of reactance (Dillard & Shen, 2005): when a message or a correction is received as a restriction of the freedom to judge, the theory predicts derogation of the source and reinforcement of the threatened position.

ATHENA does **not** rely on the "backfire effect" (Nyhan & Reifler, 2010). Large-scale replications (Wood & Porter, 2019) indicate that factual corrections do correct beliefs, without necessarily shifting attitudes. What ATHENA assesses is the perceived threat to freedom and its consequences for the source and the position, not a supposed failure of facts.

## Scope and Intended Use

ATHENA is an **analytical tool for understanding reception dynamics**. It diagnoses; it does not certify facts, and it does not predict individual behaviour.

Its operational use is currently focused on **state information defence**. It is not designed as a manipulation technique.

## Public Layer vs Private Implementation

This repository presents the **public layer** of ATHENA: concepts, architecture, workflow, doctrine and selected cases.

The following are **not published**: assessment criteria and scales, weightings, thresholds and decision rules, signal definitions, reference grids (archetypes, slides, pole frameworks), prompts, operating procedures, software tools, and case files.

This distinction is intentional.

## Versioning

| Public version | Date | Content |
|---|---|---|
| 2026.1 | 9 March 2026 | Conceptual four-pole framework |
| 2026.2 | November 2026 | Operational chain: upstream layers, reactance module, objective setting, temporal layer, epistemic doctrine, LLM-assisted workflow |

## Citation

Cahour, E. (2026). *ATHENA Framework: A Reception-Analysis Framework for Narrative Influence* (version 2026.2). GitHub repository. https://github.com/Athena-Narrative/athena-framework

## Author

ATHENA was designed and developed by **Elise Cahour** as an independent research initiative on narrative reception and psychological reactance.

## Contact

Research inquiries and collaboration proposals: elise.cahour@athena-narrative.com

## License

Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (**CC BY-NC-SA 4.0**)

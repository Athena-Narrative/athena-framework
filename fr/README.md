# Cadre ATHENA
### Un cadre d'analyse de la réception des récits d'influence

*English version: [`../README.md`](../README.md)*

ATHENA est un cadre d'analyse qui étudie **la réception des récits** : pourquoi un message est absorbé, amplifié, ignoré ou rejeté par un public donné, dans un contexte donné, à un moment donné.

ATHENA ne traite pas un récit comme un contenu persuasif isolé. Il le lit comme une **perturbation dans un système cognitif collectif**. Selon la configuration de ce système, le même récit peut prendre, stagner ou déclencher une réaction contraire.

---

## Ce que fait ATHENA

ATHENA structure l'analyse de la réception autour de **quatre pôles en interaction**.

| Pôle | Ce qu'il observe |
|---|---|
| **CORPS** | La structure narrative du message |
| **TERRAIN** | La configuration psychologique, culturelle et sociale du public |
| **BOUCLIER** | Les mécanismes de défense et la réactance psychologique |
| **VECTEUR** | Les dynamiques d'activation et de propagation |

Ensemble, ces pôles aident l'analyste à comprendre si un récit est fort, et surtout **pourquoi il fonctionne, échoue, s'enlise, polarise ou déclenche de la réactance** auprès d'un public précis.

Depuis sa première publication (mars 2026), ATHENA est passé d'un modèle conceptuel à une **chaîne d'analyse opérationnelle**, éprouvée sur des cas rétrospectifs de manipulation de l'information d'origine étrangère.

---

## L'idée centrale

ATHENA déplace l'analyse des récits de l'**analyse de contenu** vers l'**analyse de la réception**.

Le cadre aide à répondre à des questions comme :

- Pourquoi un récit apparemment fort échoue-t-il ?
- Pourquoi un récit médiocre devient-il viral ?
- À quel moment la pression narrative produit-elle de la réactance plutôt que de la persuasion ?
- Quand une dénonciation publique risque-t-elle d'amplifier le récit qu'elle vise ?
- Quelle part d'un diagnostic peut être confrontée au réel, et quelle part reste une hypothèse ?

---

## Nouveautés de la version 2026.2

Le cœur à quatre pôles est inchangé. Autour de lui, ATHENA comprend désormais :

| Composant | Rôle |
|---|---|
| **Lecture archétypale** | Couche d'identification amont : quelle figure l'émetteur incarne, quels rôles il assigne aux autres, et vers quel état (« ombre » ou « lumière ») le récit glisse. Identifiée une seule fois, sous preuve, puis partagée avec les pôles. |
| **Module réactance** | BOUCLIER est évalué par un module dédié, qui sépare la réactance portée par le message de celle portée par le contexte social du public. |
| **Substrat de réception** | Description structurée du terrain *avant* l'arrivée du message : défiance institutionnelle, polarisation, demande sociale pour certains récits. |
| **Fixation d'objectif** | Avant toute évaluation, l'analyste fixe ce que le récit cherche à obtenir (modifier une perception, installer une croyance, déclencher un comportement) et sa visée stratégique de long terme. Les pôles évaluent par rapport à cet objectif, pas dans l'absolu. |
| **Interopérabilité avec DISARM et DIMA** | Les descriptions côté attaquant (tactiques, techniques cognitives) entrent comme matériau amont. Elles éclairent l'analyse de la réception sans y être fusionnées. |
| **Couche temporelle** | Demi-vie narrative, phase narrative, distinction entre opération ponctuelle et campagne cumulative. |
| **Doctrine épistémique** | Chaque entrée porte son statut de preuve ; chaque sortie porte son régime de preuve. ATHENA dit ce qui est vérifiable et ce qui ne l'est pas. |
| **Chaîne assistée par LLM, avec humain dans la boucle** | Des modèles de langage proposent des évaluations structurées sous contrat de preuve explicite ; l'analyste arbitre, complète ce qui dépend du contexte, et valide. |
| **Sortie à deux niveaux** | Un rapport analyste, et une note sans jargon pour les décideurs. |

L'historique daté de ces développements figure dans [`CHANGELOG.md`](CHANGELOG.md).

---

## Architecture

```text
              MATÉRIAU AMONT
   Lecture archétypale · Cadres côté attaquant
   (DISARM, DIMA) · Substrat de réception
                    │
                    ▼
           FIXATION D'OBJECTIF
   Objectif narratif immédiat · Visée long terme
                    │
                    ▼
                VECTEUR
          (Activation / diffusion)
                    ▲
                    │
CORPS ◄────── Configuration du système ──────► TERRAIN
(Structure du récit)              (Configuration du public)
                    │
                    ▼
               BOUCLIER
       (Réactance / seuil de défense)
                    │
                    ▼
   VALIDATION ANALYSTE → DIAGNOSTIC → NOTE
                    │
                    ▼
        Contrôle sur observables (RETEX)
```

## Principe

L'effet d'un récit naît de l'**interaction entre des forces d'influence et des forces de résistance**.

| Influence | Résistance | Issue |
|-----------|------------|--------|
| Forte | Faible | Adoption du récit |
| Forte | Forte | Conflit / polarisation |
| Faible | Faible | Inertie informationnelle |
| Faible | Forte | Rejet défensif |

### Les configurations que cela révèle

**Les faux messages forts.** Un récit paraît convaincant mais échoue parce qu'il déclenche de fortes réactions de défense.

**Les messages faibles qui deviennent viraux.** Un récit médiocre se répand parce que tout le système est aligné : terrain réceptif, résistance faible, vecteur fort.

**Les points de bascule.** Augmenter la pression sur un public résistant aggrave la situation : dévalorisation de la source, durcissement de la position menacée, contre-mobilisation.

**L'attaque faible sur terrain fragile.** Le danger tient moins au message qu'à l'état du public qui le reçoit. Sur-réagir peut faire plus de dégâts que l'opération elle-même (voir [`cases/doppelganger-punaises-2023.md`](cases/doppelganger-punaises-2023.md)).

---

## Déroulé d'une analyse (résumé)

1. Réunir le matériau amont (lecture archétypale, description côté attaquant, substrat de réception)
2. Fixer l'objectif du récit
3. Évaluer les quatre pôles, chacun en aveugle des notes des autres
4. Compléter et valider les évaluations qui dépendent du contexte (analyste)
5. Diagnostiquer la configuration et la confronter à la lecture de l'analyste
6. Produire le rapport analyste et la note pour décideurs
7. Énoncer les observables qui confirmeraient ou infirmeraient le diagnostic

Documentation détaillée :

- [`docs/conceptual-foundations.md`](docs/conceptual-foundations.md) : fondements conceptuels
- [`docs/system-architecture.md`](docs/system-architecture.md) : architecture
- [`docs/analytical-workflow.md`](docs/analytical-workflow.md) : déroulé d'analyse
- [`docs/epistemic-doctrine.md`](docs/epistemic-doctrine.md) : doctrine épistémique
- [`docs/limitations-and-scope.md`](docs/limitations-and-scope.md) : limites et périmètre
- [`../docs/references.md`](../docs/references.md) : références (en anglais)

Cas :

- [`cases/covid-5g.md`](cases/covid-5g.md) : cas conceptuel illustratif
- [`cases/doppelganger-punaises-2023.md`](cases/doppelganger-punaises-2023.md) : cas rétrospectif, traité avec la chaîne opérationnelle

---

## Usages

- analyse des manipulations de l'information d'origine étrangère (FIMI)
- raisonnement de conception de contre-récits
- red teaming d'une communication stratégique ou de crise
- anticipation du risque de réception avant publication
- recherche sur la désinformation et la réactance

## Positionnement

ATHENA est **complémentaire** des cadres qui décrivent l'attaquant.

- **[DISARM](https://github.com/disarmfoundation)** décrit ce qui s'est passé dans une campagne d'influence (tactiques, séquence, acteurs).
- **[DIMA](https://github.com/M82-project/DIMA)**, développé par le projet M82, décrit les techniques cognitives sur lesquelles repose une manipulation.
- **ATHENA** analyse **comment le public visé est susceptible de la recevoir**, et pourquoi.

## Ancrage théorique : la réactance, pas le « backfire effect »

Le pôle de résistance d'ATHENA s'ancre dans la **théorie de la réactance psychologique** (Brehm, 1966) et dans le modèle « intertwined » de la réactance (Dillard et Shen, 2005) : lorsqu'un message ou une correction est reçu comme une restriction de la liberté de juger, la théorie prédit la dévalorisation de la source et le renforcement de la position menacée.

ATHENA ne **repose pas** sur le « backfire effect » (Nyhan et Reifler, 2010). Les réplications à grande échelle (Wood et Porter, 2019) indiquent que les corrections factuelles corrigent bien les croyances, sans nécessairement déplacer les attitudes. Ce qu'ATHENA évalue, c'est la menace perçue sur la liberté et ses conséquences pour la source et pour la position, pas un prétendu échec des faits.

## Périmètre et usage prévu

ATHENA est un **outil d'analyse pour comprendre les dynamiques de réception**. Il diagnostique ; il ne certifie pas les faits et ne prédit pas le comportement d'un individu.

Son usage opérationnel est aujourd'hui tourné en priorité vers la **défense informationnelle étatique**. Ce n'est pas une technique de manipulation.

## Couche publique et mise en œuvre privée

Ce dépôt présente la **couche publique** d'ATHENA : concepts, architecture, déroulé, doctrine et cas choisis.

Ne sont **pas publiés** : les critères et échelles d'évaluation, les pondérations, les seuils et règles de décision, la définition des signaux, les grilles de référence (archétypes, glissements, cadres de pôle), les prompts, les procédures, les outils logiciels et les dossiers.

Cette séparation est voulue.

## Versions

| Version publique | Date | Contenu |
|---|---|---|
| 2026.1 | 9 mars 2026 | Cadre conceptuel à quatre pôles |
| 2026.2 | Novembre 2026 | Chaîne opérationnelle : couches amont, module réactance, fixation d'objectif, couche temporelle, doctrine épistémique, chaîne assistée par LLM |

## Citation

Cahour, E. (2026). *ATHENA Framework: A Reception-Analysis Framework for Narrative Influence* (version 2026.2). Dépôt GitHub. https://github.com/Athena-Narrative/athena-framework

## Autrice

ATHENA a été conçu et développé par **Elise Cahour**, dans le cadre d'une recherche indépendante sur la réception des récits et la réactance psychologique.

## Contact

Demandes de recherche et propositions de collaboration : elise.cahour@athena-narrative.com

## Licence

Creative Commons Attribution - Pas d'utilisation commerciale - Partage dans les mêmes conditions 4.0 International (**CC BY-NC-SA 4.0**)

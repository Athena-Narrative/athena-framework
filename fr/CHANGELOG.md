# Journal des versions

Ce fichier consigne l'historique de développement du cadre ATHENA. Il décrit **ce qui** a été introduit et **quand**, pas la manière dont c'est mis en œuvre.

Les dates renvoient aux versions de travail internes de l'autrice. Le dépôt public est mis à jour par jalons.

*English version: [`../CHANGELOG.md`](../CHANGELOG.md)*

---

## [2026.2] — Novembre 2026

Mise à jour publique qui acte le passage du cadre conceptuel à une chaîne d'analyse opérationnelle.

### Ajouts

- **Lecture archétypale** (couche d'identification amont). Identification de la figure archétypale de l'émetteur et de son état (lumière / ombre), des rôles assignés aux autres acteurs, du glissement observé ou anticipé entre états, et de la cible implicite pour laquelle le message est taillé. Identifiée une fois par dossier, sous preuve, et partagée avec les pôles comme un fait descriptif.
- **Module réactance.** La réactance psychologique est évaluée par un module dédié, qui sépare les facteurs portés par le message de ceux portés par le contexte social et historique du public. BOUCLIER en est dérivé.
- **Substrat de réception.** Description structurée du terrain avant le message (défiance institutionnelle, polarisation, demande sociale de récits), pour que l'analyse ne soit pas centrée sur la seule offre.
- **Fixation d'objectif.** Étape explicite entre le matériau amont et l'évaluation par les pôles : l'objectif narratif immédiat et la visée stratégique de long terme sont fixés avant toute notation, pour éviter la circularité.
- **Désambiguïsation de « ça prend ».** Trois variables de sortie distinctes : modifier une perception, installer une croyance, déclencher un comportement. La variable pertinente est fixée en amont.
- **Interopérabilité avec DISARM et [DIMA](https://github.com/M82-project/DIMA) (projet M82).** Les descriptions côté attaquant entrent comme matériau amont, restent sur leur propre plan et ne sont jamais agrégées à l'évaluation côté public.
- **Couche temporelle.** Demi-vie narrative, phase narrative, et mode de dossier (ponctuel ou campagne cumulative) comme préalable de pertinence.
- **Véracité déclarée.** Chaque dossier porte un statut de véracité déclaré par l'analyste (vrai / faux / malinformation / non déclaré). ATHENA ne produit jamais ce statut. Un même niveau de résistance se lit différemment selon lui : résistance saine à un faux, ou rejet d'un message vrai.
- **Doctrine épistémique.** Contrat de preuve sur les entrées (factuel / déduit / non évaluable) et quatre régimes de preuve sur les sorties (voir `docs/epistemic-doctrine.md`).
- **Chaîne assistée par LLM, avec humain dans la boucle.** Des modèles de langage produisent des propositions structurées sous contrat de preuve ; l'analyste arbitre, complète les évaluations qui dépendent du contexte, et valide. Règle de révision unique sur les évaluations contestées.
- **Sortie à deux niveaux.** Rapport analyste et note sans jargon pour décideurs.
- **Cas rétrospectif :** Doppelganger, vague « punaises de lit », France, octobre 2023.

### Changements

- Ancrage théorique explicité : réactance psychologique (Brehm, 1966 ; Dillard et Shen, 2005), et non « backfire effect » (Nyhan et Reifler, 2010 ; voir Wood et Porter, 2019).
- Version française de la documentation publique (`fr/`).
- Repositionnement : ATHENA hiérarchise des **hypothèses de réception** ; il ne prédit pas un comportement.
- La concordance des tests rétrospectifs est redéfinie en conséquence : accord sur la hiérarchie des hypothèses retenues, pas sur un seuil comportemental.

### Jalons de développement (internes)

| Période | Jalon |
|---|---|
| Juin 2026 | Cadrage de la couche temporelle et stratégique ; définition de l'étape de fixation d'objectif |
| Juillet 2026 | Consolidation du module réactance ; triage d'observabilité des sorties (quatre régimes de preuve) ; champ de véracité déclarée ; substrat de réception |
| Octobre 2026 | Formalisation de la lecture archétypale comme couche amont ; contrat de proposition LLM et outil de saisie analyste ; premier cas rétrospectif traité de bout en bout |

---

## [2026.1] — 9 mars 2026

Première publication.

- Cadre conceptuel à quatre pôles : CORPS, TERRAIN, BOUCLIER, VECTEUR
- Matrice de diagnostic influence / résistance
- Déroulé d'analyse de base
- Cas illustratif : récit COVID-19 / 5G

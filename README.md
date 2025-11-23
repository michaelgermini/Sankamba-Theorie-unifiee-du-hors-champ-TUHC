📘 **Sankamba — Théorie unifiée du hors-champ (TUHC)**

Ce dépôt contient le projet de livre *Sankamba — Théorie unifiée du hors-champ*, ainsi que ses **RFC associées**.  
L’objectif est de proposer à la fois :

- un **texte long pédagogique** (chapitres 1 à 9) ;
- et une **formalisation technique** (RFC-0001 / RFC-0002) permettant l’implémentation, la simulation et l’annotation de cas concrets.

## Vue d’ensemble

- **Sankamba** : cadre théorique général autour du hors-champ.  
- **TUHC (Théorie Unifiée du Hors-Champ)** : cœur conceptuel, articulé en trois axes (politique, esthétique, ontologique).  
- **MULS** : langage structurel des mini-univers, utilisé comme base pour l’axe ontologique et les simulations.  
- **MML–DNF–Morse** : exemples techniques de transmission “hors-champ” (environnements contraints, off‑grid), évoqués dans les applications.

Le dépôt est pensé pour être lisible **comme un livre** mais aussi utilisable **comme une base de travail** pour des projets de recherche, d’art, de design ou d’ingénierie.

## Structure du projet

- `README.md` : présentation générale du projet, mode d’emploi rapide.
- `plan_global.md` : table des matières détaillée et notes de structure du livre.
- `RFC-0001-TUHC.md` : modèle conceptuel et terminologie de base de la TUHC (champ / hors-champ, axes P/A/O, configuration de hors-champ).
- `RFC-0002-TUHC.md` : grammaire formelle minimale, signatures `SIG(TUHC)`, définition d’`UMH` (Univers avec Hors-champ) et intégration avec MULS.
- Dossier `chapitres/` : texte complet du livre, un fichier par chapitre :
  - `chapitre_01_introduction.md` — Introduction à Sankamba et à la TUHC.
  - `chapitre_02_fondements_theoriques.md` — Fondements théoriques, perception, capitalisme attentionnel, trois axes.
  - `chapitre_03_axe_politique.md` — Axe politique : hors-champ social, pouvoir implicite, topologies invisibles.
  - `chapitre_04_axe_esthetique.md` — Axe esthétique : hors-champ perceptuel, omissions, silences, exemples artistiques.
  - `chapitre_05_axe_ontologique.md` — Axe ontologique : espace relationnel, morphs, couches, formalisation via MULS.
  - `chapitre_06_synthese_des_axes.md` — Synthèse P/A/O, définition de `SIG(TUHC)` et premiers scénarios de simulation.
  - `chapitre_07_applications_pratiques.md` — Analyses sociales, art & design, simulations, transmission, gouvernance hors-champ.
  - `chapitre_08_perspectives_extensions.md` — RFC TUHC, extensions multidimensionnelles, théorie générale du hors-champ universel.
  - `chapitre_09_annexes.md` — Glossaire, exemples de mini-univers, piste de bibliographie, remerciements.

## Comment lire / utiliser ce dépôt

### Lecture “livre” (conceptuelle)

- **Étape 1** : lire `chapitre_01_introduction.md` et `chapitre_02_fondements_theoriques.md` pour saisir le vocabulaire de base (hors-champ, axes P/A/O, TUHC, lien avec MULS).  
- **Étape 2** : enchaîner avec les chapitres 3, 4 et 5 pour explorer en détail chaque axe (politique, esthétique, ontologique).  
- **Étape 3** : lire `chapitre_06_synthese_des_axes.md` pour comprendre la notion de **signature de hors-champ** `SIG(TUHC)` et la synthèse des axes.  
- **Étape 4** : utiliser les chapitres 7 et 8 comme **boîte à outils** (applications, perspectives, liens avec MULS, MML–DNF–Morse, RFC).

### Lecture “spec” (technique)

- **Commencer par `RFC-0001-TUHC.md`** :  
  - définitions officielles de champ/hors-champ,  
  - description des axes,  
  - notion de configuration `H = (P, A, O)`.
- **Puis `RFC-0002-TUHC.md`** :  
  - morphs TUHC (`P`, `A`, `O`, `E_H`, `X_H`),  
  - opérateurs (`->`, `~>`, `<->`, `*`, `[]`),  
  - forme générale de `SIG_TUHC(...)`,  
  - définition d’`UMH` et **trois exemples complets** :
    - plateforme vidéo off-grid sobre,
    - réseau social centralisé grand public,
    - mini-univers cosmologique abstrait (cosmo / MULS pur).

Ces fichiers RFC servent de **pont** entre le texte et d’éventuelles implémentations (code, simulations, annotations de données).

## Méthodologie d'écriture / de travail

1. **Structure d'abord** :  
   - clarifier les sections, sous-sections et liens conceptuels (TUHC, MULS, MML–DNF–Morse, axes P/A/O),  
   - utiliser `plan_global.md` comme carte.
2. **Remplissage progressif** :  
   - travailler chapitre par chapitre,  
   - ancrer chaque développement dans l’un des axes, puis le reconnecter aux autres.
3. **Allers-retours théorie / exemples** :  
   - alterner formalisations, schémas, analogies et cas concrets (art, réseaux sociaux, physique, mini-univers, protocoles réseau).  
4. **Intégration des RFC** :  
   - considérer les RFC comme des “annexes vivantes”, prêtes à être révisées au fur et à mesure que la théorie se précise,  
   - utiliser la grammaire TUHC/MULS pour décrire des cas précis (UMH) rencontrés en recherche ou en pratique.

Le style visé est **pédagogique, rigoureux et technique**, en français, avec une progression du plus intuitif (perception du hors-champ) vers le plus formel (TUHC, `SIG(TUHC)`, MULS, simulations).

## État du projet

- Texte des chapitres 1 à 9 : **rédigé** (version de travail, appelant encore relectures et ajustements).  
- `RFC-0001-TUHC.md` et `RFC-0002-TUHC.md` : **brouillons structurés**, suffisamment stables pour des premières expérimentations.  
- Exemples UMH (off-grid, réseau social, cosmologique) : **prototypes conceptuels** destinés à être affinés et éventuellement implémentés.

Les contributions possibles incluent : corrections, ajouts d’exemples, propositions d’autres UMH, extensions de la grammaire TUHC ou traductions partielles dans d’autres langues.
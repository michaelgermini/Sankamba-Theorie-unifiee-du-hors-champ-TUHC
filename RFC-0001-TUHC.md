# RFC-0001 — TUHC : Modèle conceptuel et terminologie de base

Statut : **Brouillon**  
Auteurs : Sankamba Project  
Version : 0.1.0  

## 1. Objet et portée

### 1.1 Objet

Ce RFC définit le **modèle conceptuel de la Théorie Unifiée du Hors-Champ (TUHC)** et sa terminologie minimale.  
Il ne spécifie pas encore une grammaire formelle complète ni des formats de données, qui sont couverts par `RFC-0002-TUHC`.

### 1.2 Portée

La TUHC fournit un cadre pour décrire le **hors-champ** dans des systèmes :

- **esthétiques** (images, récits, interfaces, médias),  
- **sociaux et politiques** (réseaux, institutions, plateformes, gouvernance),  
- **ontologiques / structurels** (structures sous-jacentes modélisées, par ex. via MULS).

Ce RFC définit :

- la distinction **champ / hors-champ**,  
- les **trois axes principaux** (politique, esthétique, ontologique),  
- le concept général de **configuration de hors-champ**.

### 1.3 Hors de portée

Ce document **ne** :

- spécifie **aucun format d’échange** (JSON, MML, etc.),  
- ne définit pas de **signature formelle** (SIG(TUHC)),  
- ne traite pas de l’intégration détaillée avec **MULS** ou d’autres langages.

Ces aspects appartiennent à `RFC-0002-TUHC` et aux RFC ultérieurs.

## 2. Modèle général champ / hors-champ

### 2.1 Définitions

**Champ** :  
Ensemble des éléments **directement donnés** dans un système de représentation ou d’interaction, pour un observateur donné (ex. ce qui est visible à l’écran, entendu, énoncé explicitement, documenté publiquement).

**Hors-champ** :  
Ensemble des éléments **non donnés directement** dans le champ, mais qui :

- influencent, contraignent ou prolongent ce qui est dans le champ,  
- sont structurellement liés au champ (continuité, dépendance, corrélation).

### 2.2 Propriétés du hors-champ

La TUHC considère que le hors-champ est :

- **structuré** : ce n’est pas un simple vide, mais un ensemble de relations, de règles, de potentiels,  
- **modulable** : il est possible d’agir (au moins partiellement) sur le hors-champ en modifiant des cadres, des infrastructures, des topologies,  
- **multidimensionnel** : il se déploie simultanément sur plusieurs axes (politique, esthétique, ontologique, etc.).

## 3. Axes fondamentaux de la TUHC

### 3.1 Vue d’ensemble

La TUHC distingue trois **axes principaux** :

- **Axe esthétique (A)** : hors-champ perceptuel, sensible et médiatique.  
- **Axe politique (P)** : hors-champ social, pouvoir implicite, visibilité/invisibilité.  
- **Axe ontologique (O)** : hors-champ fondamental, structures sous-jacentes.

Ces axes ne correspondent pas à des domaines complètement séparés, mais à des **projections complémentaires** d’une même configuration de hors-champ.

### 3.2 Axe esthétique (A)

L’axe esthétique décrit le hors-champ en termes de :

- **cadres** (ce qui est inclus/exclu dans l’image, la scène, l’interface),  
- **ellipses** et **silences** (ce qui est omis de manière signifiante),  
- **indices** et **signes implicites** (ce qui renvoie à un dehors non montré).

Le hors-champ esthétique est ce que le sujet :

- **perçoit** sans que ce soit explicitement donné,  
- **reconstruit** via imagination, mémoire, attentes.

### 3.3 Axe politique (P)

L’axe politique décrit le hors-champ comme :

- **configuration de pouvoir implicite** (décisions, alliances, normes hors de l’espace public),  
- **distribution de la visibilité et de l’invisibilité**,  
- **capacité de retrait, d’opacité, de contrôle du cadre**.

Il s’applique en particulier aux :

- réseaux sociaux, plateformes, médias,  
- institutions, organisations, infrastructures de gouvernance.

### 3.4 Axe ontologique (O)

L’axe ontologique décrit le hors-champ comme :

- **structure fondamentale** du réel ou du système modélisé,  
- ensemble de **relations primaires**, de **couches** et de **topologies** sous-jacentes,  
- base à partir de laquelle émergent les phénomènes observables.

Cet axe est naturellement lié à des langages structurels tels que **MULS**.

## 4. Configurations de hors-champ

### 4.1 Triplet (P, A, O)

Pour un système donné, la TUHC considère une **configuration de hors-champ** comme un triplet :

\( H = (P, A, O) \)

où :

- **P** : décrit la composante politique du hors-champ (pouvoir implicite, visibilité, retrait, opacité),  
- **A** : décrit la composante esthétique (cadres, omissions, indices perceptifs),  
- **O** : décrit la composante ontologique (structure profonde, morphs, couches, topologies).

Les composantes peuvent être décrites :

- qualitativement (récits, schémas, analyses),  
- ou, dans des RFC ultérieures, quantitativement (vecteurs, signatures, paramètres).

### 4.2 Couplages entre axes

La TUHC postule que les composantes P, A, O sont **couplées** :

- des décisions esthétiques (A) peuvent renforcer ou atténuer des configurations politiques (P),  
- des structures ontologiques (O) rendent possibles ou impossibles certaines mises en scène (A) et distributions du pouvoir (P),  
- des reconfigurations politiques (P) peuvent modifier les structures ontologiques (O) (ex. changement d’infrastructures).

Ces couplages feront l’objet d’une formalisation explicite dans `RFC-0002-TUHC`.

## 5. Niveaux de description

### 5.1 Niveau descriptif

Au premier niveau, la TUHC opère comme :

- un **cadre de description** :  
  - on décrit où se situent les hors-champs esthétique, politique et ontologique,  
  - on identifie les zones blanches, les acteurs implicites, les structures invisibles.

### 5.2 Niveau structurel

Au second niveau, la TUHC vise :

- la production de **schémas, graphes, cartes** du hors-champ,  
- l’identification de **morphs**, de **liens** et de **couches** (en particulier via MULS pour l’axe ontologique).

### 5.3 Niveau formel et opératoire

Les niveaux formel (signatures, grammaire) et opératoire (simulation, implémentation) sont introduits mais **non spécifiés** dans ce RFC.  
Ils constituent l’objet principal de `RFC-0002-TUHC`.

## 6. Terminologie minimale

Ce RFC définit et réserve, pour la TUHC :

- **TUHC** : Théorie Unifiée du Hors-Champ.  
- **Champ / Hors-champ** : au sens de la section 2.1.  
- **Axes P, A, O** : politique, esthétique, ontologique.  
- **Configuration de hors-champ** : triplet \(H = (P, A, O)\).  
- **Couplage d’axes** : interaction entre composantes P, A, O.  
- **Sankamba** : nom du cadre global englobant TUHC, MULS, MML–DNF–Morse et les applications associées.

## 7. Considérations de sécurité et d’éthique

Bien que ce RFC soit conceptuel, l’usage de la TUHC soulève des questions :

- **Sur-modélisation** : risque de réduire des réalités complexes à des schémas trop simples.  
- **Exposition du hors-champ** : rendre visible certains hors-champs (sociaux, politiques, intimes) peut mettre en danger des individus ou des groupes.  
- **Neutralisation critique** : la formalisation ne doit pas servir à naturaliser ou justifier des configurations de pouvoir.

Toute application de la TUHC devrait expliciter :

- les **enjeux éthiques** liés à la cartographie du hors-champ,  
- les **limites** au-delà desquelles il est préférable de préserver des zones d’opacité et d’autonomie.

## 8. Références

- Sankamba, *Théorie unifiée du hors-champ* (chapitres 1–3 pour les bases conceptuelles, 5–6 pour l’axe ontologique et la synthèse).  
- `RFC-0001-MULS` — *Le Langage Structurel des Mini-Univers (MULS)*.  
- `RFC-0002-TUHC` — *Grammaire formelle, signatures SIG(TUHC) et intégration avec MULS* (brouillon, à paraître).



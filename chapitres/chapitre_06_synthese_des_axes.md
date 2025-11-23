# Chapitre 6 : Synthèse des axes

Après avoir détaillé séparément les trois axes de Sankamba — politique, esthétique, ontologique — ce chapitre propose une **synthèse**.  
Il montre comment un même hors-champ peut être situé simultanément sur plusieurs plans, comment la TUHC permet de modéliser ces configurations, et introduit la notion de **signature de hors-champ** (SIG(TUHC)), base des simulations à venir.

## 6.1 Interconnexion entre politique, esthétique et ontologie

### 6.1.1 Un même phénomène, trois projections

Un même dispositif peut être lu selon les trois axes de la TUHC :

- **Esthétique** : comment il cadre l’expérience sensible (ce qui est montré, suggéré, tu),  
- **Politique** : comment il distribue la visibilité, le pouvoir, la possibilité de retrait,  
- **Ontologique** : quelles structures profondes (relations, couches, topologies) le rendent possible.

Prenons un exemple simplifié : une **plateforme de vidéos**.

- Sur l’axe esthétique :  
  - choix de cadrage des vidéos, de mise en page, de hiérarchie des contenus ;  
  - hors-champ perceptuel : vidéos non recommandées, commentaires masqués, zones d’écran vides ou surchargées.
- Sur l’axe politique :  
  - qui apparaît dans les recommandations ? avec quelle fréquence ?  
  - quels comptes sont invisibilisés, déréférencés, suspendus ?  
  - quels acteurs contrôlent ces paramètres ?
- Sur l’axe ontologique :  
  - architecture du système (serveurs, bases de données, algorithmes),  
  - topologie des flux (comment circulent données et signaux),  
  - mini-univers MULS sous-jacents (structures de liens, couches d’abstraction).

Le **hors-champ** de cette plateforme n’est donc pas seulement ce que l’utilisateur ne voit pas à l’écran :  
c’est l’ensemble **esthétique + politique + ontologique** qui conditionne ce qu’il peut voir, dire et faire.

### 6.1.2 Cartographie croisée des axes

On peut représenter un hors-champ donné comme un **point** ou une **région** dans un espace à trois dimensions (P, A, O) :

- **P** (politique) : degré de retrait, d’opacité, de pouvoir implicite,  
- **A** (esthétique) : intensité des omissions, densité d’indices, usage des silences,  
- **O** (ontologique) : profondeur et complexité des structures invisibles (liens, couches, intrication).

Un phénomène peut alors être caractérisé par un **vecteur** :

\( H = (P, A, O) \)

où chaque composante peut être, selon le cas, qualitative (description) ou quantitative (score, indicateur).  
Cette représentation ne prétend pas capturer toute la richesse du réel, mais fournit un **outil de comparaison** et de modélisation.

### 6.1.3 Effets de couplage

Les axes ne sont pas indépendants :

- des choix esthétiques (A) peuvent renforcer ou atténuer des structures politiques (P),  
- des structures ontologiques (O) peuvent rendre certains cadres esthétiques ou politiques impossibles,  
- des reconfigurations politiques (P) peuvent transformer les structures ontologiques (O) (par exemple en modifiant les infrastructures).

La TUHC s’intéresse à ces **effets de couplage** :  
comment une décision apparemment locale (changer un cadrage, un paramètre algorithme, un protocole) résonne sur les trois axes simultanément.

## 6.2 Modélisation d’un TUHC complet

### 6.2.1 Qu’est-ce qu’un TUHC complet ?

Un **TUHC complet** est une modélisation explicite d’une situation de hors-champ qui :

- identifie les trois axes (P, A, O) en jeu,  
- spécifie les principales variables pertinentes pour chacun,  
- décrit les relations entre ces variables,  
- et, idéalement, permet de **simuler** ou **tester** des transformations (que se passe-t-il si l’on modifie telle couche ontologique, tel paramètre de visibilité, tel dispositif esthétique ?).

Il ne s’agit pas de tout modéliser, mais de :

- isoler une **configuration de hors-champ** donnée,  
- et d’en proposer une **carte structurée**.

### 6.2.2 Niveaux de description

On peut distinguer plusieurs niveaux dans la modélisation d’un TUHC complet :

1. **Niveau descriptif** :  
   - récit, analyse qualitative, repérage des hors-champs sur chaque axe.
2. **Niveau structurel** :  
   - schémas, graphes, diagrammes, identification de morphs, de liens, de couches (inspirés de MULS).
3. **Niveau formel** :  
   - introduction de signatures (SIG), vecteurs, paramètres, éventuellement équations ou règles logiques.
4. **Niveau opérationnel** :  
   - simulation, mise en œuvre technique (mini-univers MULS, infrastructures comme MML–DNF–Morse, protocoles de test).

Un même cas peut être abordé à ces différents niveaux, selon les besoins :  
conceptualisation, écriture, recherche, expérimentation.

### 6.2.3 Paramètres d’un modèle TUHC

Sans prétendre à l’exhaustivité, un modèle TUHC complet inclura typiquement :

- **Pour l’axe politique (P)** :  
  - distribution de la visibilité, du retrait, de l’opacité, du contrôle du cadre, de l’influence implicite ;  
  - nature des acteurs et de leurs relations (ouverts/fermés, centraux/périphériques).
- **Pour l’axe esthétique (A)** :  
  - types de cadres, d’ellipses, de silences ;  
  - densité d’indices, modes de suggestion ;  
  - trajectoires du regard/attention.
- **Pour l’axe ontologique (O)** :  
  - nombre et types de morphs,  
  - configuration des liens,  
  - couches et topologies (MULS).

Ces paramètres nourriront ensuite la définition d’une **signature** de hors-champ.

## 6.3 SIG(TUHC) : signature d’un hors-champ

### 6.3.1 Intuition de la signature

La notion de **signature** est empruntée à MULS (signature d’univers) et adaptée à la TUHC.  
L’idée est de condenser, pour un hors-champ donné, un ensemble minimal d’informations qui :

- caractérise sa **structure**,  
- permet de le **comparer** à d’autres,  
- et ouvre à la **simulation**.

La signature ne remplace pas la description détaillée, mais joue le rôle d’un **résumé structurel**.

### 6.3.2 Forme générale de SIG(TUHC)

On peut proposer une forme générique :


SIG_TUHC(P, A, O, L, C, χ_H)


où, à titre indicatif :

- **P** : paramètres politiques agrégés (par exemple, un vecteur ou un score global),  
- **A** : paramètres esthétiques (types d’ellipses, densité d’indices, régime de silence),  
- **O** : paramètres ontologiques (par exemple, signature MULS associée : Ns, Nb, Nc, Deff, χ),  
- **L** : niveau de **liaison** entre axes (force des couplages P–A, A–O, P–O),  
- **C** : complexité perçue du hors-champ (nombre de couches, degré d’intrication),  
- **χ_H** : un invariant global propre au hors-champ (par analogie à la caractéristique d’Euler, mais à définir pour la TUHC).

Cette notation volontairement abstraite sera spécifiée et diversifiée selon les cas d’étude.

### 6.3.3 Exemple conceptuel

Considérons un cas simplifié :

- une œuvre audiovisuelle qui traite d’un sujet sensible,  
- diffusée sur une plateforme contrôlée,  
- avec une infrastructure technique centralisée.

On peut imaginer une signature du type :


SIG_TUHC(
  P = {V_distribuée, R_faible, O_inégale, C_fort, I_élevée},
  A = {ellipses fortes, silences marqués, indices denses},
  O = SIG_MULS(Ns=10, Nb=3, Nc=2, Deff=4, χ=1),
  L = {P–A:fort, A–O:moyen, P–O:fort},
  C = élevé,
  χ_H = +1
)


Ce pseudo-exemple montre comment on peut **emboîter** :

- la signature MULS dans la composante O,  
- et des agrégats qualitatifs/quantitatifs pour P et A.

## 6.4 Exemples chiffrés et simulations

### 6.4.1 Vers des modèles numériques

À partir des signatures SIG(TUHC), il devient possible de :

- construire des **modèles numériques** (graphes, réseaux de neurones structurés, automates) qui incarnent certaines configurations de hors-champ,  
- explorer comment des modifications de paramètres (P, A, O, L, C, χ_H) affectent la dynamique observable.

Même si ces modèles restent simplifiés, ils peuvent :

- servir de **laboratoires conceptuels**,  
- éclairer des intuitions,  
- générer des scénarios extrêmes ou inattendus.

### 6.4.2 Rôle de MULS et des mini-univers

MULS intervient ici comme **moteur de simulation ontologique** :

- en définissant des mini-univers précis (configurations de morphs, liens, couches),  
- en associant à chaque mini-univers une **signature d’univers** (SIG(MULS)),  
- en couplant ces mini-univers avec des paramètres P et A dans la signature SIG(TUHC).

On peut ainsi :

- concevoir des univers où le hors-champ ontologique est très complexe mais où le champ phénoménal semble simple,  
- ou l’inverse : univers où le champ semble chaotique alors que la structure profonde est régulière.

Ces expériences conceptuelles aident à penser :

- les écarts entre ce que l’on voit, ce qui est socialement en jeu, et ce qui est structurellement à l’œuvre.

### 6.4.3 Scénarios exploratoires

Parmi les scénarios possibles :

- **Augmentation de l’opacité politique (P)** sans modifier la structure ontologique (O) :  
  - que devient la perception du système par ses acteurs ?  
  - quels effets sur la confiance, la lisibilité, la capacité d’action ?
- **Modification d’une couche ontologique (O)** (par exemple, changement de topologie MULS) à P et A constants :  
  - certains comportements émergents apparaissent-ils ou disparaissent-ils ?  
  - comment cela se traduit-il dans le champ perceptif ?
- **Réécriture esthétique (A)** d’un système inchangé en profondeur (O, P constants) :  
  - que se passe-t-il si l’on modifie les cadres, les ellipses, les formes de mise en scène sans toucher à la structure ?  
  - jusqu’où peut-on “reconfigurer” le hors-champ perçu sans changer le hors-champ ontologique ?

Ces scénarios montrent que la TUHC n’est pas seulement une théorie descriptive, mais un **outil d’exploration** :  
elle permet de formuler des hypothèses, de les tester mentalement ou via des modèles, et d’ouvrir un espace de réflexion critique sur la place du hors-champ dans nos univers esthétiques, sociaux et structurels.

---

Avec ce chapitre, la TUHC dispose d’un **noyau synthétique** :  
les trois axes sont articulés, un cadre de modélisation est posé, et la notion de SIG(TUHC) offre un langage pour résumer et comparer des structures de hors-champ.  
Les chapitres suivants se tourneront vers les **applications pratiques** (analyse sociale, art, simulation, transmission) et les **perspectives formelles** (RFC, intégration poussée avec MULS et MML–DNF–Morse).


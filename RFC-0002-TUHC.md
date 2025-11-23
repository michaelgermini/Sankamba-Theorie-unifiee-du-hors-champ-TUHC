# RFC-0002 — TUHC : Grammaire formelle, signatures SIG(TUHC) et intégration MULS

Statut : **Brouillon**  
Auteurs : Sankamba Project  
Version : 0.1.0  
Dépend de : `RFC-0001-TUHC`, `RFC-0001-MULS`

## 1. Objet et portée

### 1.1 Objet

Ce RFC spécifie :

- une **grammaire formelle minimale** pour décrire des configurations de hors-champ dans la TUHC,  
- la notion de **signature de hors-champ** (`SIG(TUHC)`),  
- les principes d’**intégration** avec le langage structurel des mini-univers (`MULS`).

### 1.2 Portée

Le document définit :

- des **types de morphs TUHC**,  
- des **opérateurs de relation** entre morphs,  
- un format conceptuel de signature `SIG_TUHC(P, A, O, L, C, χ_H)`,  
- un schéma d’**emboîtement** de signatures TUHC dans des signatures MULS (et inversement).

Il ne prescrit pas encore de format d’encodage unique (JSON, MML, etc.), mais propose une **notation ASCII** de référence.

## 2. Modèle TUHC formel

### 2.1 Morphs TUHC

La TUHC introduit des **morphs** de hors-champ, analogues aux morphs de MULS, mais orientés vers les trois axes P, A, O :

- `P` — morph politique (pouvoir implicite, visibilité, retrait, opacité, contrôle de cadre).  
- `A` — morph esthétique (cadre, omission, indice, silence, trajectoire perceptive).  
- `O` — morph ontologique (structure profonde, lien, couche, topologie).  
- `E_H` — morph d’intrication de hors-champ (liaison forte entre morphs TUHC).  
- `X_H` — morph d’interaction multiple de hors-champ (configurations complexes, croisées).

> Note : ces morphs sont logiques/conceptuels et peuvent être mappés sur des morphs MULS (`S`, `B`, `C`, `E`, `X`, `T`) dans les intégrations TUHC–MULS.

### 2.2 Objets TUHC

On appelle **objet TUHC** toute entité décrite par un ensemble de morphs et de liens sur les axes P, A, O.  
Exemples : un acteur social, une plateforme, une œuvre, un protocole, un mini-univers, une interface.

## 3. Opérateurs et relations

### 3.1 Opérateurs binaires

Les opérateurs suivants sont utilisés pour relier des morphs :

- `->` : **influence directe** (un morph agit explicitement sur un autre).  
- `~>` : **effet implicite / latéral** (relation indirecte, contexte, halo).  
- `<->` : **intrication** (relation bi-directionnelle forte, corrélation structurelle).  
- `*` : **interaction multiple** (composition de plusieurs morphs en configuration).  
- `[]` : **couche** (appartenance à un layer donné).

Ces opérateurs ne sont pas limités à un seul axe :  
des relations `P -> A`, `A ~> O`, `P <-> O` sont permises.

### 3.2 Exemple de micro-grammaire

Exemple conceptuel (non normatif) :

```text
HCH {
  P:"acteur_visible"    -> A:"mise_en_scene"
  A:"ellipse_violence" ~> P:"perception_pouvoir"
  O:"structure_reseau" <-> P:"capteur_donnees"
  E_H:"liaison_esth_polit" : (A1, P1)
  X_H*(P1, A1, O1)
}
```

Cet exemple illustre :

- un morph politique influençant un morph esthétique (`P -> A`),  
- un morph esthétique ayant des effets latents sur le politique (`A ~> P`),  
- une intrication entre structure ontologique et captation de données (`O <-> P`),  
- une interaction multiple croisant les trois axes (`X_H*(P, A, O)`).

## 4. Signatures SIG(TUHC)

### 4.1 Intuition

Une **signature de hors-champ** `SIG(TUHC)` condense, pour une configuration donnée :

- la composition politique (P),  
- la composition esthétique (A),  
- la composition ontologique (O),  
- le niveau de couplage entre axes (L),  
- la complexité globale (C),  
- un invariant de hors-champ (`χ_H`).

Elle ne remplace pas les descriptions détaillées, mais fournit un **résumé structurel**.

### 4.2 Forme générale

Forme abstraite proposée :

```text
SIG_TUHC(
  P = P_conf,
  A = A_conf,
  O = O_conf,
  L = L_conf,
  C = C_level,
  χ_H = chi_H
)
```

où :

- `P_conf` : ensemble ou vecteur de paramètres politiques (visibilité, retrait, opacité, contrôle, influence implicite).  
- `A_conf` : ensemble ou vecteur de paramètres esthétiques (cadres, ellipses, densité d’indices, régimes de silence, trajectoires d’attention).  
- `O_conf` : paramètres ontologiques, **incluant typiquement une signature MULS** (ex. `SIG_MULS(Ns, Nb, Nc, Deff, χ)`).  
- `L_conf` : paramètres de liaison P–A, A–O, P–O (par ex. qualitativement : faible/moyen/fort ; quantitativement : coefficients).  
- `C_level` : niveau de complexité perçue ou structurelle du hors-champ.  
- `chi_H` : invariant global propre à la configuration de hors-champ (à définir par usage ; peut être un scalaire, un symbole de classe, etc.).

### 4.3 Exemple semi-formel

```text
SIG_TUHC(
  P = { V=0.8, R=0.2, O=0.3, C=0.7, I=0.9 },
  A = { ellipses="fortes", silences="marqués", indices="denses" },
  O = SIG_MULS(Ns=10, Nb=3, Nc=2, Deff=4, χ=1),
  L = { P_A="fort", A_O="moyen", P_O="fort" },
  C = "élevé",
  χ_H = +1
)
```

Ce format n’est pas un encodage machine définitif, mais un **schéma conceptuel** que des formats concrets (JSON, MML, YAML, etc.) peuvent implémenter.

## 5. Intégration avec MULS

### 5.1 Rappel : SIG(MULS)

`RFC-0001-MULS` définit la signature d’un mini-univers :

```text
SIG(Ns, Nb, Nc, Deff, χ)
```

avec :

- `Ns` : nombre de cordes (S),  
- `Nb` : nombre de branes (B),  
- `Nc` : nombre de dimensions compactifiées (C),  
- `Deff` : dimensions effectives,  
- `χ` : caractéristique topologique globale.

### 5.2 Mini-univers avec hors-champ (UMH)

On appelle **UMH** (Univers avec Hors-champ) une structure combinant :

- une signature MULS (structure ontologique),  
- une signature TUHC (hors-champ complet).

Forme conceptuelle :

```text
UMH {
  SIG_MULS(Ns, Nb, Nc, Deff, χ)
  SIG_TUHC(P, A, O, L, C, χ_H)
  // Morphs MULS (S, B, C, E, X, T, ...)
  // Morphs TUHC (P, A, O, E_H, X_H, ...)
  // Liens entre couches MULS et TUHC
}
```

L’UMH permet de :

- lier explicitement une **structure ontologique** (MULS) et des **configurations de hors-champ** sur les autres axes,  
- fournir un support à des **simulations** (par exemple, via code MULS + annotations TUHC).

### 5.3 Mapping TUHC ↔ MULS

Il est recommandé, sans que ce soit strictement normatif, d’établir un mapping de travail :

- morphs `O` ↔ morphs MULS (`S`, `B`, `C`, `T`),  
- morphs `E_H` ↔ morphs `E` (intrication),  
- morphs `X_H` ↔ morphs `X` (interactions multiples),  
- couches TUHC ↔ couches MULS (`Layer_HCH`, `Layer_Spatial`, etc.).

Exemple illustratif :

```text
UMH {
  SIG_MULS(3,1,2,4,1)
  SIG_TUHC(P=..., A=..., O=SIG_MULS(3,1,2,4,1), L=..., C=..., χ_H=...)

  // Couche spatiale (MULS)
  S:"s1":(C1,C2)
  B:"b1":(s1)
  C:"d1":()

  // Couche hors-champ politique
  [Layer_P]
  P:"acteur_A" -> P:"acteur_B"

  // Couplage
  E_H:"liaison_O_P" : (O1, P1)
}
```

## 6. Notation ASCII de référence

### 6.1 Objectifs

La notation ASCII de référence doit :

- être **lisible par l’humain**,  
- être **facilement parseable**,  
- pouvoir être **transmise sur des canaux contraints** (y compris via MML–DNF–Morse).

### 6.2 Esquisse de notation

Un bloc TUHC minimal peut être représenté ainsi :

```text
HCH {
  P:"acteur_visible"    -> A:"mise_en_scene"
  A:"ellipse_violence"  ~> P:"perception_pouvoir"
  O:"structure_reseau"  <-> P:"collecte_donnees"

  SIG_TUHC(
    P={V=0.8,R=0.2,O=0.3,C=0.7,I=0.9},
    A={ellipses="fortes",silences="marqués"},
    O=SIG_MULS(10,3,2,4,1),
    L={P_A="fort",A_O="moyen",P_O="fort"},
    C="élevé",
    χ_H=+1
  )
}
```

Cette notation :

- n’est pas un standard binaire,  
- mais une **cible sémantique** pour d’éventuels encodeurs/décodeurs (y compris sur des couches comme MML–DNF–Morse).

## 7. Considérations d’implémentation

### 7.1 Formats de données

Les implémentations peuvent choisir des formats variés :

- JSON / YAML / TOML pour les utilisations logicielles,  
- MML (Minimal Markup Language) pour les transmissions en environnements contraints,  
- formats spécifiques pour des outils de simulation (graphes, DSL, etc.).

Il est recommandé de :

- préserver une **isomorphie claire** avec la sémantique de ce RFC,  
- documenter explicitement les mappings entre formats locaux et structures TUHC.

### 7.2 Interopérabilité

L’interopérabilité entre implémentations nécessite au minimum :

- une **compréhension commune** des morphs TUHC (`P`, `A`, `O`, `E_H`, `X_H`),  
- une représentation explicite de `SIG_TUHC`,  
- un mécanisme pour référencer des signatures MULS (`SIG_MULS`) lorsque l’axe ontologique est utilisé.

## 8. Considérations de sécurité et d’éthique

La formalisation de hors-champs sensibles (politiques, sociaux, intimes) peut :

- exposer des **zones de vulnérabilité**,  
- être utilisée pour **optimiser des dispositifs de contrôle** ou de manipulation,  
- contribuer à une **objectivation indésirable** de vécus ou de structures.

Les implémentations de TUHC devraient :

- respecter des **principes d’anonymisation et de minimisation** lorsqu’elles traitent des données réelles,  
- expliciter les **usages attendus et non souhaités**,  
- inclure, lorsque pertinent, des **garde-fous** techniques et organisationnels (journalisation, audit, consentement).

## 9. Exemple complet d’UMH (Univers avec Hors-champ)

### 9.1 Contexte : plateforme vidéo distribuée en environnement contraint

Cet exemple illustre un **UMH** modélisant une plateforme de diffusion vidéo légère, opérant :

- sur une infrastructure **off-grid** (réseau local + radio, via MML–DNF–Morse),  
- avec une interface minimaliste, pensée pour préserver le hors-champ perceptuel (éviter la saturation),  
- sous un régime politique où certaines décisions de classement et de modération sont prises hors du champ public.

L’objectif est de montrer :

- la **structure ontologique** (MULS),  
- la **signature de hors-champ** (TUHC),  
- et quelques **liaisons explicites** entre couches.

### 9.2 Composant MULS : structure ontologique simplifiée

```text
UMH {
  // Signature MULS de l’univers technique sous-jacent
  SIG_MULS(
    Ns=4,     // 4 "cordes" : canaux de transport (Wi-Fi local, radio Morse, stockage local, synchronisation différée)
    Nb=2,     // 2 "branes" : couches logicielles (DNF réseau, couche application vidéo)
    Nc=1,     // 1 dimension compactifiée : métadonnées minimales (MML) non visibles comme telles
    Deff=3,   // 3 dimensions effectives : temps, espace réseau, graphe des nœuds
    χ=1       // topologie globalement connectée, un seul composant
  )

  // Morphs MULS (esquisse)
  S:"canal_wifi"    : (C1)
  S:"canal_morse"   : (C1)
  S:"stockage_local": ()
  S:"sync_differee" : (C1)

  B:"DNF_layer"     : ( "canal_wifi", "canal_morse" )
  B:"APP_video"     : ( "DNF_layer", "stockage_local", "sync_differee" )

  C:"meta_MML"      : ()
}
```

Ici, la signature MULS encode :

- des **canaux de transport** (S),  
- des **couches logicielles** (B),  
- une **dimension compactifiée** pour les métadonnées minimales (C).

Cette structure est le **hors-champ ontologique** de l’expérience utilisateur : elle n’apparaît pas directement, mais conditionne la diffusion des vidéos.

### 9.3 Composant TUHC : signature de hors-champ

On décrit maintenant la configuration de hors-champ à l’aide de `SIG_TUHC` :

```text
  SIG_TUHC(
    P = { 
      V=0.7,   // visibilité moyenne des créateurs locaux
      R=0.6,   // capacité réelle de retrait (déconnexion possible, stockage local)
      O=0.5,   // opacité partielle des critères de recommandation
      C=0.4,   // contrôle du cadre réparti (communauté + opérateurs)
      I=0.8    // forte influence implicite via choix des nœuds relais
    },
    A = { 
      cadres="sobres", 
      ellipses="modérées", 
      indices="parcellaires", 
      silences="présents" 
    },
    O = SIG_MULS(4,2,1,3,1),   // on réutilise explicitement la signature MULS ci-dessus
    L = { 
      P_A="fort",   // les décisions politiques influencent fortement l’esthétique (mise en avant, modération)
      A_O="moyen",  // l’esthétique est partiellement contrainte par l’architecture technique
      P_O="fort"    // certaines décisions politiques (choix des relais, des canaux) modifient l’architecture
    },
    C = "élevé",    // complexité globale importante (plusieurs couches + couplages)
    χ_H = +1        // invariant de hors-champ : configuration orientée vers la résilience et la sobriété
  )
```

Cette signature résume :

- l’état du hors-champ politique (distribution de la visibilité, retrait, opacité, contrôle, influence),  
- l’état du hors-champ esthétique (style de l’interface, usage des ellipses et silences),  
- le hors-champ ontologique (structure MULS),  
- et la force des couplages entre ces niveaux.

### 9.4 Liens explicites entre morphs MULS et morphs TUHC

On ajoute enfin quelques relations TUHC dans l’UMH :

```text
  // Couche hors-champ politique
  [Layer_P]
  P:"noeud_relais"        -> P:"visibilite_createurs"
  P:"groupe_moderation"   -> P:"filtrage_contenus"

  // Couche hors-champ esthétique
  [Layer_A]
  A:"interface_sobre"     ~> P:"perception_equite"
  A:"absence_compteurs"   ~> P:"deplacement_attention"

  // Couche hors-champ ontologique (référencée à MULS)
  [Layer_O]
  O:"archi_MULS" <-> B:"APP_video"

  // Couplages de hors-champ (intrication)
  E_H:"politique_archi" : (P:"groupe_moderation", O:"archi_MULS")
  E_H:"esth_politique"  : (A:"interface_sobre",   P:"perception_equite")

  // Interaction multiple globale
  X_H*( P:"noeud_relais", A:"interface_sobre", O:"archi_MULS" )
}
```

Commentaires :

- `P:"noeud_relais" -> P:"visibilite_createurs"` : certains nœuds du réseau ont un rôle central dans la diffusion, ce qui crée un hors-champ politique de la visibilité.  
- `A:"absence_compteurs" ~> P:"deplacement_attention"` : une décision esthétique (ne pas afficher de compteurs de vues) a des effets politiques implicites sur la manière dont la reconnaissance circule.  
- `O:"archi_MULS" <-> B:"APP_video"` : intrication entre la structure MULS et le comportement apparent de l’application.  
- `E_H` et `X_H` modélisent comment ces dimensions sont intimement liées, sans apparaître comme telles dans l’interface.

### 9.5 Résumé

Cet UMH fournit :

- une **signature MULS** (structure ontologique de l’univers technique),  
- une **signature TUHC** (configuration de hors-champ politique, esthétique et ontologique),  
- un ensemble de **liens explicites** entre morphs MULS et morphs TUHC.

Il peut servir de base :

- à des **simulations** (en faisant varier certains paramètres et en observant les effets),  
- à des **discussions conceptuelles** (par exemple sur la visibilité, la sobriété, la résilience),  
- à des **implémentations expérimentales** (prototypes de plateformes off-grid).

## 10. Deuxième exemple d’UMH : réseau social centralisé grand public

### 10.1 Contexte

Cet exemple illustre un UMH représentant un **réseau social centralisé** grand public, où :

- l’infrastructure est fortement centralisée (data centers, CDN, protocole unique),  
- l’interface est saturée d’éléments de visibilité (compteurs, recommandations, flux infini),  
- de nombreuses décisions de classement et de modération sont opaques pour les utilisateurs.

L’objectif est de contraster avec l’exemple précédent (plateforme off-grid sobre) en montrant une **autre signature de hors-champ**.

### 10.2 Composant MULS : structure centralisée

```text
UMH_CENTRAL {
  SIG_MULS(
    Ns=6,     // multiples canaux : mobile, web, APIs, tracking, CDN, ads
    Nb=3,     // branes : couche API, couche recommandation, couche interface
    Nc=2,     // dimensions compactifiées : profils de tracking, scoring caché
    Deff=4,   // temps, graphe des utilisateurs, graphe de contenus, graphe d’annonces
    χ=1
  )

  S:"canal_web"      : (C1)
  S:"canal_mobile"   : (C1)
  S:"canal_tracking" : (C2)
  S:"canal_ads"      : (C2)
  S:"cdn"            : ()
  S:"storage"        : ()

  B:"API_layer"      : ( "canal_web", "canal_mobile" )
  B:"reco_layer"     : ( "API_layer", "canal_tracking" )
  B:"ui_layer"       : ( "reco_layer", "cdn", "storage" )

  C:"profil_tracking": ()
  C:"profil_scoring" : ()
}
```

### 10.3 Composant TUHC : signature de hors-champ

```text
  SIG_TUHC(
    P = {
      V=0.95,  // très forte visibilité des contenus conformes au modèle de la plateforme
      R=0.2,   // faible capacité de retrait effectif (données persistantes, difficulté à disparaître)
      O=0.9,   // forte opacité des algorithmes et des critères de modération
      C=0.9,   // contrôle du cadre très concentré (entreprise centrale)
      I=0.95   // influence implicite très élevée (architecture + normes)
    },
    A = {
      cadres="denses",
      ellipses="faibles",
      indices="surchargés",
      silences="raréfiés"   // peu de zones blanches, flux quasi continu
    },
    O = SIG_MULS(6,3,2,4,1),
    L = {
      P_A="très_fort",
      A_O="fort",
      P_O="très_fort"
    },
    C = "très_élevé",
    χ_H = -1          // invariant de hors-champ orienté vers la capture attentionnelle
  )
```

### 10.4 Liens entre couches

```text
  [Layer_P]
  P:"entreprise_centrale"  -> P:"normes_visibilite"
  P:"normes_visibilite"    -> P:"reputation_utilisateurs"

  [Layer_A]
  A:"flux_infini"          ~> P:"dilution_signal"
  A:"compteurs_visibilite" ~> P:"course_aux_metrics"

  [Layer_O]
  O:"reco_graph" <-> B:"reco_layer"
  O:"profil_scoring" <-> S:"canal_ads"

  E_H:"couplage_politique_tech" : (P:"entreprise_centrale", O:"reco_graph")
  E_H:"couplage_esth_polit"     : (A:"compteurs_visibilite", P:"reputation_utilisateurs")

  X_H*( P:"entreprise_centrale", A:"flux_infini", O:"profil_scoring" )
}
```

### 10.5 Lecture comparative avec l’exemple off-grid

Comparé à l’UMH de la plateforme vidéo off-grid (section 9) :

- la **structure MULS** est plus riche en canaux et en couches centrées (tracking, ads, CDN),  
- la signature `P` montre une **concentration du contrôle** et une **faible capacité de retrait**,  
- la signature `A` indique une **saturation du champ perceptif**,  
- `χ_H` prend un signe opposé, symbolisant un régime de hors-champ orienté vers la **capture** plutôt que vers la résilience.

Ces deux UMH forment un **diptyque conceptuel** : ils ne couvrent pas toutes les possibilités, mais tracent un spectre entre des architectures de hors-champ plus sobres/émancipatrices et des architectures plus captatives/centrées.

## 11. Troisième exemple d’UMH : mini-univers cosmologique abstrait

### 11.1 Contexte

Ce troisième exemple illustre un UMH **purement cosmologique / structurel** :  
il ne représente ni plateforme technique, ni système social explicite, mais un **mini-univers MULS** pensé comme :

- un espace doté de dimensions visibles et compactifiées,  
- plusieurs types de morphs (cordes, branes, intrication, interactions multiples),  
- un hors-champ ontologique riche, auquel on associe une lecture TUHC minimale (O dominant, P et A quasi latents).

L’objectif est de montrer comment la TUHC peut être appliquée à un univers **sans interface ni acteurs sociaux explicites**, en se concentrant sur l’axe ontologique et sur une interprétation cosmologique.

### 11.2 Composant MULS : mini-univers E/X-Type

```text
UMH_COSMO {
  SIG_MULS(
    Ns=5,     // 5 cordes (modes de propagation fondamentaux)
    Nb=2,     // 2 branes (régions / "membranes" d’univers)
    Nc=3,     // 3 dimensions compactifiées (micro-structure)
    Deff=4,   // 4 dimensions effectives (par ex. 3 d’espace + 1 de temps)
    χ=2       // caractéristique topologique non triviale (deux composantes reliées)
  )

  // Cordes fondamentales
  S:"s1":(C1)
  S:"s2":(C2)
  S:"s3":(C3)
  S:"s4":(C1,C2)
  S:"s5":(C2,C3)

  // Branes (régions d’univers)
  B:"brane_A":("s1","s2","s4")
  B:"brane_B":("s3","s5")

  // Dimensions compactifiées
  C:"dim_c1":()
  C:"dim_c2":()
  C:"dim_c3":()

  // Intrications et interactions multiples
  E:"ent_pair":("s2","s5")
  X:"interaction_cluster":("s1","s3","s4","s5")
}
```

Cet univers :

- possède deux “régions” (branes A et B) reliées par des intrications et interactions multiples,  
- inclut trois dimensions compactifiées qui ne sont pas directement accessibles à un observateur macroscopique,  
- présente une topologie globale non triviale (χ=2).

### 11.3 Composant TUHC : lecture cosmologique

On associe à ce mini-univers une signature TUHC où l’axe ontologique domine :

```text
  SIG_TUHC(
    P = {
      V=0.0,   // pas d’acteurs sociaux explicites
      R=0.0,
      O=0.0,
      C=0.0,
      I=0.0
    },
    A = {
      cadres="implicites",      // le cadre est ici fourni par la structure MULS elle-même
      ellipses="structurelles", // l’observateur ne perçoit qu’une partie de la structure
      indices="topologiques",
      silences="ontologiques"
    },
    O = SIG_MULS(5,2,3,4,2),
    L = {
      P_A="nul",
      A_O="moyen",   // l’esthétique d’un univers perçu (si on le projetait) serait contrainte par O
      P_O="nul"
    },
    C = "élevé",
    χ_H = 0          // invariant de hors-champ neutre : univers de référence pour la TUHC ontologique
  )
```

Ici :

- `P` est nul par construction (aucune couche politique explicite),  
- `A` est interprété de manière virtuelle : si un observateur percevait cet univers, son expérience serait marquée par de fortes ellipses structurelles (accès partiel à la topologie réelle),  
- `O` reprend `SIG_MULS`, affirmant que le hors-champ est essentiellement ontologique.

### 11.4 Liens interprétatifs

On peut, à titre de lecture TUHC, relier certains morphs MULS à des concepts esthétiques potentiels :

```text
  [Layer_O]
  O:"topologie_global" <-> T:"χ=2"

  [Layer_A_virtuel]
  A:"horizon_observable" ~> O:"brane_A"
  A:"phenomenes_inexpliques" ~> E:"ent_pair"
  A:"asymetries" ~> X:"interaction_cluster"
}
```

Ces liens ne décrivent pas une interface concrète, mais :

- la manière dont un observateur interne, limité à certaines régions ou échelles, pourrait **éprouver** le hors-champ ontologique (phénomènes inexpliqués, asymétries, horizons),  
- comment des propriétés topologiques profondes (χ=2, intrication, dimensions compactifiées) deviennent des **indices** ou des **silences** au niveau phénoménal.

Ce troisième UMH sert ainsi de **cas-limite** :

- un univers où la presque totalité du hors-champ est ontologique,  
- et où P et A ne sont envisagés que comme **projections possibles** d’un observateur hypothétique, plutôt que comme couches déjà réalisées.

## 12. Références

- `RFC-0001-TUHC` — *Modèle conceptuel et terminologie de base*.  
- `RFC-0001-MULS` — *Le Langage Structurel des Mini-Univers (MULS)*.  
- Sankamba, *Théorie unifiée du hors-champ* (chapitres 5–8 pour l’axe ontologique et les perspectives cosmologiques).

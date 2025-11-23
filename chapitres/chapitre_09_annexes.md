# Chapitre 9 : Annexes

Ce chapitre rassemble les **ressources de référence** nécessaires pour naviguer dans Sankamba : un glossaire des principaux termes, des indications de codes d’exemples, une bibliographie minimale et des remerciements.

## 9.1 Glossaire des termes MULS et TUHC

**Axe esthétique (TUHC)**  
Plan d’analyse du hors-champ centré sur l’expérience sensible : ce qui est montré, omis, suggéré, les ellipses, les silences, les cadres (chapitres 2 et 4).

**Axe ontologique (TUHC)**  
Plan d’analyse du hors-champ comme structure fondamentale de la réalité : relations primaires, morphs, couches, topologies (chapitres 2 et 5).  

**Axe politique (TUHC)**  
Plan d’analyse du hors-champ social et du pouvoir implicite : visibilité/invisibilité, retrait, opacité, topologies invisibles (chapitres 2 et 3).

**Champ / Hors-champ**  
Le champ désigne ce qui est donné, visible, directement accessible ; le hors-champ désigne ce qui n’apparaît pas mais influence, contraint ou prolonge le champ (chapitres 1 et 2).

**Hors-champ perceptuel**  
Ensemble des éléments suggérés, supposés, reconstruits dans une expérience esthétique ou médiatique : ce que le sujet perçoit sans que ce soit montré explicitement (chapitre 4).

**Hors-champ social**  
Configurations de pouvoir, d’influence et de relations qui ne se donnent pas comme telles dans l’espace public, mais structurent les possibles d’un système social (chapitre 3).

**Hors-champ ontologique**  
Niveau profond de relations, de morphs et de couches qui rend possible l’espace phénoménal sans être directement observable (chapitre 5).

**MULS (Mini-Universe Language Structural)**  
Langage formel pour décrire des mini-univers par leurs structures (morphs, liens, couches, signatures), servant de base à l’axe ontologique de la TUHC.

**Morphs (MULS)**  
Briques élémentaires de MULS (S, B, C, E, X, T, etc.) représentant des entités structurelles (cordes, branes, dimensions compactifiées, intrication, interactions multiples, topologies) (chapitre 5).

**Couches / Layers (MULS/TUHC)**  
Plans distincts de structure ou de réalité (micro/macro, visible/invisible, technique/social) pouvant être reliés, intriqués ou partiellement disjoints (chapitres 2, 5 et 6).

**Intrication (E)**  
Relation structurelle forte entre entités qui ne peuvent être décrites indépendamment ; modèle d’un hors-champ de corrélation (chapitre 5).

**SIG(MULS)**  
Signature d’un mini-univers MULS : \(SIG(Ns, Nb, Nc, Deff, χ)\), qui condense le nombre de morphs de chaque type, les dimensions effectives et un invariant topologique global (chapitre 5).

**SIG(TUHC)**  
Signature d’un hors-champ dans le cadre de la TUHC : résumé structurel des composantes politiques, esthétiques et ontologiques, incluant leurs couplages et un invariant global χ_H (chapitre 6).

**TUHC (Théorie unifiée du hors-champ)**  
Cadre proposé par Sankamba pour penser, modéliser et simuler le hors-champ à travers plusieurs axes reliés, en lien avec MULS et d’autres systèmes (ensemble de l’ouvrage).

**Sankamba**  
Nom donné au projet théorique qui articule TUHC, MULS, pratiques esthétiques, analyse sociale et architectures techniques, en plaçant le hors-champ au centre.

## 9.2 Codes d’exemples mini-univers

Cette section indique des **schémas types** et fragments de pseudo-code permettant de construire des mini-univers MULS illustrant différentes formes de hors-champ.

**Mini-univers simple (S-Type)**  
Illustration d’un univers où quelques cordes (S) sont reliées de manière minimale, montrant comment une structure très simple peut déjà produire un hors-champ ontologique (chapitre 5).

```text
UNIVERSE {
  SIG(3,0,0,1,1)
  S:"s1":()
  S:"s2":(s1)
  S:"s3":(s1,s2)
}
```

**Mini-univers avec dimensions compactifiées (C-Type)**  
Exemple d’un univers avec dimensions non directement observables (C), permettant de travailler l’intuition des “dimensions cachées” comme hors-champ ontologique (chapitre 5).

```text
UNIVERSE {
  SIG(2,1,2,3,0)
  S:"s1":(C1)
  S:"s2":(C2)
  B:"b1":(s1,s2)
  C:"d1":()
  C:"d2":()
}
```

**Mini-univers intriqué (E-Type)**  
Univers dans lequel des morphs E modélisent l’intrication : utile pour explorer le lien entre corrélations invisibles et phénomènes émergents (chapitres 5 et 6).

```text
UNIVERSE {
  SIG(2,0,0,1,1)
  S:"a":()
  S:"b":()
  E:"pair":("a","b")
}
```

**Couplage TUHC–MULS (UMH)**  
Schémas combinant une signature MULS et une signature TUHC pour représenter un mini-univers avec hors-champ intégré (UMH), base des expérimentations du chapitre 7.

Dans une version ultérieure (RFC et dépôt de code associé), ces exemples pourront être fournis comme :  
- fichiers MULS annotés,  
- scripts de simulation,  
- visualisations interactives.

## 9.3 Bibliographie et références

Cette section regroupe quelques **repères** pour situer Sankamba dans un paysage plus large, sans prétendre épuiser les références possibles.

**Sur le hors-champ et l’esthétique**  
- Travaux sur le hors-champ cinématographique et les théories de l’image.  
- Réflexions sur le silence, l’ellipse, le hors-texte en littérature et en arts visuels.  

**Sur les médias, le capitalisme attentionnel et les réseaux sociaux**  
- Analyses du capitalisme de plateforme, de l’économie de l’attention, de la logique des flux continus.  
- Études sur la visibilité, l’invisibilité sociale, l’opacité et la résistance dans les environnements numériques.

**Sur les systèmes complexes et la théorie des systèmes**  
- Ouvrages sur l’émergence, les dynamiques multi-couches, la résilience des systèmes distribués.  

**Sur la physique théorique, l’espace et l’émergence**  
- Textes de vulgarisation ou travaux théoriques sur les dimensions cachées, l’émergence de l’espace, les topologies globales.  

**Sur MULS, MML–DNF–Morse et les RFC associées**  
- Spécification MULS (RFC-0001) : concepts, grammaire, exemples de mini-univers.  
- Documentation MML–DNF–Morse : transmission en environnements contraints, compression structurelle, protocoles off-grid.  
- Brouillons de RFC TUHC (0002 et suivants), en lien avec le présent ouvrage.

## 9.4 Remerciements et contributions

Sankamba est un projet qui se situe à la croisée de plusieurs mondes :  
théorie, écriture, modélisation, expérimentation technique.  
Il doit beaucoup :

- aux **lectrices et lecteurs** qui acceptent de prendre le hors-champ au sérieux, comme quelque chose de plus qu’un simple “manque” décoratif ;  
- aux **chercheuses et chercheurs**, aux **artistes**, aux **ingénieurs** dont les travaux sur l’espace, les réseaux, les images, les mini-univers et les transmissions en environnements contraints ont nourri ce cadre ;  
- aux **communautés techniques et open source** qui rendent possibles des langages comme MULS ou MML–DNF–Morse, et qui montrent qu’une autre approche de l’infrastructure est possible ;  
- aux **interlocuteurs critiques** qui rappellent que toute théorie du hors-champ a elle-même son hors-champ, et qu’aucun cadre ne peut prétendre capturer l’entièreté de ce qui échappe.

Ce livre peut être lu comme une **première carte** d’un territoire beaucoup plus vaste.  
Il ne demande qu’à être repris, contesté, prolongé — dans d’autres livres, d’autres codes, d’autres pratiques, peut-être aussi dans des espaces qui, par choix, resteront pour toujours hors du champ.


# 📘 Sankamba — Théorie unifiée du hors-champ (TUHC)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub issues](https://img.shields.io/github/issues/michaelgermini/Sankamba-Theorie-unifiee-du-hors-champ-TUHC)](https://github.com/michaelgermini/Sankamba-Theorie-unifiee-du-hors-champ-TUHC/issues)
[![GitHub stars](https://img.shields.io/github/stars/michaelgermini/Sankamba-Theorie-unifiee-du-hors-champ-TUHC)](https://github.com/michaelgermini/Sankamba-Theorie-unifiee-du-hors-champ-TUHC/stargazers)

> **Cadre théorique et technique pour penser, modéliser et analyser le "hors-champ"** — ce qui échappe à la visibilité directe mais structure notre réalité sociale, esthétique et ontologique.

Ce dépôt contient le manuscrit complet du livre *Sankamba — Théorie unifiée du hors-champ* ainsi que ses spécifications techniques RFC. Il offre une approche duale :

- **📖 Texte narratif pédagogique** : 9 chapitres explorant les concepts de façon progressive
- **🔧 Formalisation technique** : RFC pour implémenter et simuler des configurations de hors-champ

## 📋 Table des matières

- [Vue d'ensemble](#-vue-densemble)
- [Installation et utilisation](#-installation-et-utilisation)
- [Structure du projet](#-structure-du-projet)
- [Guide de lecture](#-guide-de-lecture)
- [Contribuer](#-contribuer)
- [Licence](#-licence)
- [Remerciements](#-remerciements)

## 🔍 Vue d'ensemble

**Sankamba** propose un cadre unifié pour analyser et formaliser le concept de "hors-champ" — ces éléments qui structurent notre réalité sans être directement visibles ou accessibles.

### Composants principaux

- **📚 TUHC (Théorie Unifiée du Hors-Champ)** : Cœur conceptuel articulé autour de trois axes fondamentaux
  - Axe **politique** : pouvoir implicite, structures sociales invisibles
  - Axe **esthétique** : perception subliminale, omissions artistiques
  - Axe **ontologique** : structures fondamentales de la réalité

- **🧬 MULS (Mini-Universe Language Structural)** : Langage formel pour décrire les structures ontologiques

- **📡 MML–DNF–Morse** : Exemples d'architectures techniques implémentant des principes de hors-champ

### Public cible

- **Chercheurs** en sciences sociales, philosophie, design
- **Artistes** et créateurs explorant les limites de la perception
- **Ingénieurs** travaillant sur des systèmes distribués ou contraints
- **Développeurs** intéressés par les langages formels et simulations

## 🚀 Installation et utilisation

### Prérequis

- Aucun prérequis technique particulier pour lire le manuscrit
- Pour les simulations : Python 3.8+, bibliothèques de graphes (NetworkX) et visualisation (Matplotlib)

### Installation

```bash
# Cloner le dépôt
git clone https://github.com/michaelgermini/Sankamba-Theorie-unifiee-du-hors-champ-TUHC.git
cd Sankamba-Theorie-unifiee-du-hors-champ-TUHC

# (Optionnel) Créer un environnement virtuel pour les simulations
python -m venv venv
source venv/bin/activate  # Sur Windows: venv\Scripts\activate
pip install -r requirements.txt  # Si un fichier requirements.txt est ajouté
```

## 📁 Structure du projet

```
Sankamba-Theorie-unifiee-du-hors-champ-TUHC/
├── 📖 chapitres/                    # Manuscrit du livre (9 chapitres)
│   ├── chapitre_01_introduction.md
│   ├── chapitre_02_fondements_theoriques.md
│   ├── chapitre_03_axe_politique.md
│   ├── chapitre_04_axe_esthetique.md
│   ├── chapitre_05_axe_ontologique.md
│   ├── chapitre_06_synthese_des_axes.md
│   ├── chapitre_07_applications_pratiques.md
│   ├── chapitre_08_perspectives_extensions.md
│   └── chapitre_09_annexes.md
├── 📋 RFC-0001-TUHC.md             # Modèle conceptuel TUHC
├── 🔧 RFC-0002-TUHC.md             # Grammaire formelle et signatures
├── 📝 plan_global.md               # Table des matières détaillée
├── 📄 README.md                    # Ce fichier
├── 🗂️ .gitignore                   # Fichiers ignorés par Git
└── 🔬 examples/                    # (À venir) Scripts et simulations
```

## 📖 Guide de lecture

### Parcours "Livre" (Approche narrative)

Idéal pour découvrir les concepts de façon progressive :

1. **Introduction** (`chapitre_01`, `chapitre_02`) : Vocabulaire de base et fondements théoriques
2. **Axes fondamentaux** (`chapitre_03-05`) : Exploration détaillée des axes politique, esthétique et ontologique
3. **Synthèse** (`chapitre_06`) : Intégration des axes et signatures TUHC
4. **Applications** (`chapitre_07-08`) : Cas pratiques et perspectives futures

### Parcours "Spécifications" (Approche technique)

Pour les implémenteurs et chercheurs :

1. **RFC-0001-TUHC.md** : Définitions conceptuelles et modèle de base
2. **RFC-0002-TUHC.md** : Grammaire formelle, signatures et exemples UMH
3. **Chapitre 9** : Glossaire et exemples de mini-univers

### Utilisations avancées

- **Simulation** : Utiliser les signatures TUHC pour modéliser des systèmes complexes
- **Annotation** : Appliquer le cadre TUHC à l'analyse de données ou œuvres
- **Extension** : Proposer de nouveaux morphs ou opérateurs pour des domaines spécifiques

## 🤝 Contribuer

### Types de contributions

Nous accueillons diverses formes de contributions :

- **📝 Corrections et améliorations** : Améliorations du texte, corrections typographiques
- **🔬 Extensions théoriques** : Nouveaux exemples UMH, morphs TUHC, applications
- **💻 Implémentations** : Scripts de simulation, visualisations, outils basés sur TUHC
- **🌐 Traductions** : Versions dans d'autres langues
- **📊 Recherche** : Études empiriques utilisant le cadre TUHC

### Processus de contribution

1. **Fork** le dépôt
2. **Créez** une branche pour votre contribution (`git checkout -b feature/amazing-feature`)
3. **Committez** vos changements (`git commit -m 'Add amazing feature'`)
4. **Poussez** vers votre fork (`git push origin feature/amazing-feature`)
5. **Ouvrez** une Pull Request

### Lignes directrices

- Respectez le style pédagogique et technique du manuscrit
- Pour les ajouts théoriques, référencez les sources appropriées
- Testez les modifications sur plusieurs chapitres pour assurer la cohérence

### Contact

- 📧 Email : michael@germini.info
- 🐛 Issues : [GitHub Issues](https://github.com/michaelgermini/Sankamba-Theorie-unifiee-du-hors-champ-TUHC/issues)
- 💬 Discussions : Section discussions du dépôt

## 📊 État du projet

- ✅ **Chapitres 1-9** : Rédigés et structurés
- ✅ **RFC TUHC** : Spécifications complètes avec exemples
- 🚧 **Simulations** : Prototypes conceptuels (à développer)
- 📈 **Communauté** : Ouvert aux contributions

## 📄 Licence

Ce projet est distribué sous licence **MIT**. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

```
Copyright (c) 2025 Michael Germini

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

## 🙏 Remerciements

**Sankamba** est le fruit d'une réflexion interdisciplinaire. Merci aux :

- **Communauté académique** pour l'inspiration théorique
- **Chercheurs en sciences sociales** pour les analyses du pouvoir invisible
- **Artistes et designers** pour l'exploration des limites perceptuelles
- **Développeurs open source** pour les outils techniques
- **Contributeurs** pour leur engagement dans ce projet

---

*Dans l'immensité du visible, le hors-champ révèle la structure profonde de nos mondes.*
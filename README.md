# 📊 Architecture de CV Dynamique Pilotée par la Donnée

[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-2f81f7?style=for-the-badge)](https://azzouzmezlini.github.io/mon-cv/)

Ce dépôt héberge mon CV interactif de **Data Engineer / Développeur SQL & Data**. Conçu selon les principes de l'architecture logicielle moderne, ce projet sépare strictement les données métiers, la structure, la logique d'IHM et les feuilles de style modulaires.

---

## 🛠️ Stack Technique & Architecture

- **Data Engine :** `cv-data.json` (Source de vérité unique stockant les données du parcours).
- **Logique Application (JavaScript ES6) :** 
  - `app.js` (Point d'entrée principal et initialisation)
  - `renderers.js` (Moteur de rendu dynamique du DOM)
  - `interactivity.js` (Gestion des interactions et des filtres)
  - `theme.js` & `config.js` (Gestion du mode clair/sombre et paramètres globaux)
- **Styles Modulaires :** 
  - `style-base.css` (Variables globales, thèmes, structure et composants de base)
  - `style-mobile.css` (Adaptations responsives spécifiques)
  - `style-print.css` (Mise en page A4 stricte, liens et QR Code pour impression/PDF)
- **Ressources :** Dossier `assets/` (éléments graphiques et médias).
- **Hébergement :** `GitHub Pages` avec intégration et déploiement continus.

---

## 🏗️ Structure du Projet

```text
mon-cv/
├── assets/
├── js/
│   ├── app.js
│   ├── config.js
│   ├── interactivity.js
│   ├── renderers.js
│   └── theme.js
├── style/
│   ├── style-base.css
│   ├── style-mobile.css
│   └── style-print.css
├── cv-data.json
├── index.html
├── LICENSE
└── README.md
```

---

## 🚀 Fonctionnalités Clés

- **Filtres & Interactivité :** Filtrage dynamique par compétences et mise en valeur interactive (*highlighting*) au survol des expériences et projets.
- **Gestion des Vues & Thèmes :** Bascule à la volée entre vue compacte et complète, combinée à un switch de thème Clair/Sombre anti-FOUC.
- **Export PDF & Impression Papier Optimisés :**
  - Liens hypertextes directs et cliquables vers LinkedIn, GitHub, la version web et les projets.
  - Masquage des éléments interactifs et intégration d'un QR Code unique pointant vers la version web interactive à l'impression.
- **En-tête Flexbox à 2 niveaux :** Séparation ergonomique entre les coordonnées de contact interactives et les informations administratives.

---

## ⚙️ Comment faire évoluer le contenu ?

Grâce au découplage complet entre les données et le code, aucune modification HTML ou CSS n'est nécessaire pour mettre à jour votre CV :

1. Ouvrez et éditez le fichier `cv-data.json`.
2. Mettez à jour ou ajoutez vos éléments dans les tableaux correspondants.
3. Validez avec un `git commit` et un `git push`.
4. GitHub Pages met à jour le site en ligne automatiquement.

---

## 🔗 Liens et Contact

- **Démo en ligne :** [Consulter mon CV sur GitHub Pages](https://azzouzmezlini.github.io/mon-cv/)
- **LinkedIn :** [Profil LinkedIn](https://www.linkedin.com/in/azzouz-mezlini)
- **GitHub :** [Profil GitHub](https://github.com/AzzouzMezlini)

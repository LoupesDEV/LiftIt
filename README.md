
<div align="center">
   <img src="https://m3-markdown-badges.vercel.app/stars/9/3/LoupesDEV/LiftConfig">
   <img src="https://ziadoua.github.io/m3-Markdown-Badges/badges/HTML/html3.svg">
   <img src="https://ziadoua.github.io/m3-Markdown-Badges/badges/CSS/css3.svg">
   <img src="https://ziadoua.github.io/m3-Markdown-Badges/badges/Javascript/javascript3.svg">
   <img src="https://ziadoua.github.io/m3-Markdown-Badges/badges/JSON/json3.svg">
</div>

# LIFT - Config

Application web légère pour configurer et estimer une configuration simracing (bundles, cockpits, sièges et accessoires).

## Table des matières

- [Présentation](#présentation)
- [Comment utiliser](#comment-utiliser)
- [Fonctionnalités](#fonctionnalités)
- [Démonstration locale](#démonstration-locale)
- [Structure du projet](#structure-du-projet)
- [Contribuer](#contribuer)

## Présentation

LIFT - Config est une interface client simple pour construire une configuration simracing en sélectionnant un bundle, un cockpit, un siège et des accessoires. L'application calcule le total estimé, conserve la sélection dans le navigateur (LocalStorage) et propose un résumé clair.

L'interface est conçue pour être utilisée directement dans le navigateur sans backend nécessaire.

## Comment utiliser

1. Cloner le dépôt :

```bash
git clone https://github.com/LoupesDEV/LiftConfig.git
```

2. Ouvrir l'application :

- Avec **VSCode** : clic-droit sur `index.html` → *Open with Live Server* (extension recommandée).
- Avec **Python** (serveur local simple) :

```powershell
python -m http.server 8000
# puis ouvrir http://localhost:8000
```

3. Naviguer dans l'interface, sélectionner les éléments souhaités et consulter le résumé dans le panneau de droite.

## Fonctionnalités

- **Sélection simple** : Choix d'un bundle, d'un cockpit, d'un siège et d'accessoires.
- **Sélection multiple pour accessoires** : Ajouter/supprimer plusieurs accessoires.
- **Résumé dynamique** : Aperçu instantané de la sélection (noms et prix).
- **Calcul du total** : Somme automatique des articles sélectionnés.
- **Persistance côté client** : Sauvegarde de la configuration dans `localStorage` pour reprise ultérieure.
- **Réinitialisation** : Bouton pour remettre la configuration à zéro.
- **Liens produits** : Les cartes peuvent contenir un lien vers la page du produit (ouverture dans un nouvel onglet).

## Démonstration locale

Après avoir lancé un serveur local, ouvrez `index.html` dans votre navigateur (par exemple `http://localhost:8000`). L'interface charge `data.json` pour peupler les cartes. Si le fichier `data.json` est absent ou mal formé, un message d'erreur s'affichera.

## Structure du projet

```
LiftConfig/
├── index.html          # Page principale
├── data.json           # Données des bundles, cockpits, sièges, accessoires
├── script.js           # Logique de rendu, sélection et sauvegarde
├── styles.css          # Styles de l'interface
└── README.md           # Documentation (ce fichier)
```

# Contributeurs

Merci aux personnes et ressources ayant contribué au projet:

- [LoupesDEV](https://github.com/LoupesDEV) — Développement principal, conception et maintenance.

Vous souhaitez contribuer ? Consultez le [guide de contribution](CONTRIBUTING.md) ou ouvrez une *issue* pour proposer
des améliorations.

<p align="center">
    <img alt="Footer" src="https://i.imgur.com/9Ojjug7.png">
    <br><br>
    <img src="https://ziadoua.github.io/m3-Markdown-Badges/badges/LicenceGPLv3/licencegplv33.svg">
</p>

# XR Dataset Exploration

## Description du système simulé
Ce projet Unity permet d'explorer un dataset simple représenté par des objets 3D interactifs.  
Chaque cube représente une ligne du CSV avec des catégories (A, B, C) et une valeur associée.  
L'objectif est de permettre à l'utilisateur de **visualiser, sélectionner et filtrer les données** pour mieux comprendre la structure du dataset avant toute analyse approfondie.  
Le système simule un **environnement XR data-driven**, idéal pour la supervision ou le monitoring simplifié.

## Mode XR choisi
- VR simulée : interaction via **souris et clavier**  
- Aucun casque VR nécessaire  
- L'utilisateur peut interagir avec les objets et les boutons de filtrage directement dans la scène Unity.

## Fonctionnalités implémentées
1. **Génération dynamique des cubes** à partir d'un fichier CSV (`dataset.csv`)  
2. **Couleurs selon la catégorie** :  
   - Catégorie A → Bleu  
   - Catégorie B → Vert  
   - Catégorie C → Rouge  
   - Cube sélectionné → Jaune  
3. **Sélection d’un cube** avec affichage d’informations via TextMeshPro  
4. **Filtrage basique par catégorie** grâce aux boutons UI : Tous / Catégorie A / B / C  
5. Architecture modulaire avec :  
   - `DataManager` → création et gestion des DataObjects  
   - `FilterManager` → filtrage et affichage des objets  
   - `InteractionManager` → sélection et mise en évidence  
6. Interface utilisateur simple avec **feedback visuel et textuel**.

## Répartition du travail
- **Sara Malki** :  
  - Création du dataset CSV  
  - Scripts `DataManager`, `InteractionManager`, `FilterManager`  
  - Préparation des matériaux et prefab `DataObject`  
  - Mise en place des boutons UI et du Canvas  
  - Tests et validation de l’exploration visuelle  

- **Meryem Benaammi** :  
  - Support dans la conception des interactions  
  - Assistance pour la mise en place des couleurs et feedback visuel  
  - Relecture et validation finale du projet  

## Compte rendu
- Le projet permet d’explorer visuellement les données d’un CSV simple dans Unity  
- Les interactions permettent de filtrer et sélectionner les cubes, avec un **feedback immédiat**  
- Architecture claire, modulable et prête pour extension (animations, AR, VR)  
- Version GitHub prête avec **Assets, Packages et ProjectSettings**, sans dossiers générés automatiquement (Library, Temp, Logs, UserSettings)

## Objectif du projet

L'objectif de ce projet est de développer un pipeline de traitement d'images aériennes pour détecter automatiquement les bâtiments à partir d'images satellites haute résolution. 

Le projet est divisé en deux étapes majeures :
- **Segmentation sémantique** des bâtiments avec un modèle de Deep Learning (U-Net).
- **Polygonisation** des masques prédis afin d'obtenir des contours vectoriels exploitables.

Le travail a été mené dans le cadre du module *Modélisation systèmes vision*.

## Données utilisées

Les données utilisées proviennent du jeu de données public **INRIA Aerial Image Labeling Dataset**.

- Résolution spatiale : 0.3 m/pixel
- Taille des images : 5000x5000 pixels (découpées en sous-patches 256x256 pour l'entraînement)
- 5 villes américaines différentes sont représentées (Austin, Chicago, Kitsap County, Western Tyrol, Vienna)

**Lien vers les données officielles :**  
🔗 [INRIA Aerial Image Labeling Dataset](https://project.inria.fr/aerialimagelabeling/)

Les annotations disponibles sont des masques binaires où les bâtiments sont représentés en blanc.

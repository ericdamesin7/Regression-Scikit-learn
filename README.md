# Projet  
# Prédiction du Poids des Poissons (Régression)

Ce projet consiste en la **construction et l’évaluation de modèles de régression** afin de prédire le **poids de poissons** à partir de leurs **caractéristiques physiques** (longueurs, hauteur, largeur) et de leur **espèce**.

Le dataset utilisé est un jeu de données classique disponible sur Kaggle, souvent utilisé pour l’apprentissage de la **régression supervisée**.

Lien du dataset :  
https://www.kaggle.com/datasets/vipullrathod/fish-market

## Pourquoi s'intéresse-t-on à prédire le poids de poissons ? Quel impact aura-il sur le business ?

On s’intéresse à la prédiction du poids des poissons car le poids détermine directement leur prix sur le marché. Pouvoir estimer ce poids sans peser chaque poisson permet de gagner du temps, de réduire la manipulation et d’automatiser des processus comme le tri et la facturation, ce qui a un impact direct sur l’efficacité et la rentabilité des activités de pêche et d’aquaculture. Par ailleurs, le poids constitue un indicateur clé de la santé des poissons, de la qualité de leur environnement et de la disponibilité de nourriture, ce qui permet de suivre la croissance des espèces et de détecter d’éventuelles anomalies liées à la pollution ou à la surpêche, contribuant ainsi à une meilleure gestion des ressources.

Bien que ce projet ait avant tout un objectif d’entraînement, on peut imaginer qu’un travail similaire, appliqué à un jeu de données beaucoup plus large et plus représentatif, puisse être développé et mis en application pour aider les pêcheurs, les aquaculteurs ou les usines de tri, notamment pour l’estimation des stocks, le tri automatique et la fixation des prix. Dans le cadre de ce projet toutefois, cette application reste purement théorique : le modèle n’est pas destiné à être déployé en production et sert uniquement à l’apprentissage des concepts de régression en machine learning.

---

L’objectif principal de ce projet est de **comprendre et appliquer les concepts fondamentaux du machine learning**, notamment :
- la régression :
    - linéaire
    - polynomiale
    - avec des arbres et des forêts aléatoires
- la validation croisée (cross-validation)
- l’analyse de l’overfitting

---

## Description du projet

Le notebook `fish.ipynb` contient :

- Analyse exploratoire des données (EDA)
- Nettoyage des données :
  - suppression des poids nuls
  - gestion des variables catégorielles
- Analyse des corrélations
- Implémentation de modèles de régression
- Utilisation de `PolynomialFeatures`
- Mise en place de **pipelines scikit-learn**
- Validation croisée (cross-validation)
- Comparaison des erreurs Train / CV
- Analyse des **feature importances** (Random Forest)

---

## Comment exécuter le projet

1. Cloner le dépôt :

```bash
git clone https://github.com/<ericdamesin7>/Regression-Scikit-learn.git
```

2. Installer les dépendances :

```bash
pip install numpy pandas matplotlib scikit-learn
```

3. Ouvrir le notebook :

```bash
jupyter notebook fish.ipynb
```

4. Exécuter les cellules dans l’ordre pour reproduire l’analyse et les résultats.

---

## Structure du projet

```
Regression-Scikit-learn/
│
├── fish-market/
│   └── Fish.csv          # Dataset brut
│
├── fish.ipynb            # Notebook principal (EDA + régression)
└── README.md             # Documentation du projet
```

---

## Auteur

* [Eric Damesin](https://github.com/ericdamesin7)
* Ce projet fait partie de mon apprentissage en **Machine Learning**.

Voici quelques visualisations de ce projet :

<img width="850" height="557" alt="image" src="https://github.com/user-attachments/assets/4fb84932-94e9-407d-8076-83a315e27c2b" />

<img width="1634" height="1470" alt="image" src="https://github.com/user-attachments/assets/6f3ea34b-e4d9-4940-b500-7c44a08eaaed" />

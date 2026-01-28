# 🧠 Travaux Pratiques de Machine Learning - 4GI

Bienvenue dans ce dépôt regroupant l'ensemble des travaux pratiques de Machine Learning. Ce projet a pour but de vous guider à travers les différentes étapes du cycle de vie d'un projet ML, de la préparation des données jusqu'au déploiement de modèles complexes.

---

## 🚀 Installation Rapide

**Prérequis :** Avoir [Python 3.9+](https://www.python.org/downloads/) installé.

1.  **Récupérer le projet :**
    ```bash
    git clone https://github.com/Nate-n23/TPs-de-ML_4GI.git
    cd TPs-de-ML_4GI
    ```

2.  **Installer les outils nécessaires :**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Lancer les notebooks :**
    ```bash
    jupyter notebook
    ```

---

## 📂 Contenu des TPs

Voici une vue d'ensemble pour comprendre rapidement ce que contient chaque session :

### [TP1 : Introduction aux Pipelines ML](TP1.ipynb)
**Objectif :** Prédire le prix de logements en Californie.
*   **Ce qu'on y fait :** Nettoyage des données, visualisation géographique, et création d'un premier modèle (Random Forest).
*   **Notions clés :** Préparation de données, Feature Engineering, Score $R^2$.

### [TP2 : Régression Avancée & MLOps](TP2.ipynb)
**Objectif :** Maîtriser la régression et la mise en production.
*   **Ce qu'on y fait :** Comparaison de modèles (Ridge vs Lasso), suivi des expériences avec MLflow et conteneurisation avec Docker.
*   **Notions clés :** Sur-apprentissage (Overfitting), Régularisation, MLOps.

### [TP3 : Apprentissage Non-Supervisé](TP3.ipynb)
**Objectif :** Découvrir des structures cachées dans les données (Clustering).
*   **Ce qu'on y fait :** Segmentation client avec K-Means et GMM, et réduction de dimension pour visualiser les données (PCA, t-SNE).
*   **Notions clés :** Clustering, Silhouette Score, Visualisation 2D/3D.

### [TP4 : Classification Médicale & Incertitude (EDL)](TP4.ipynb)
**Objectif :** Diagnostiquer des pathologies et quantifier l'incertitude des prédictions.
*   **Ce qu'on y fait :** Comparaison de modèles probabilistes (Naive Bayes, KNN) sur données synthétiques et simulation/étude théorique du *Evidential Deep Learning* (EDL).
*   **Notions clés :** Classification, K-NN, Incertitude (Aléatoire/Epistémique), Théorie de Dempster-Shafer.

---

## 🛠 Structure du Projet

*   `TP1.ipynb` à `TP4.ipynb` : Les cours interactifs et exercices.
*   `requirements.txt` : Liste des librairies à installer.
*   `mlruns/` : Dossier de suivi des expériences (MLflow).
*   `*.pkl / *.onnx` : Modèles entraînés sauvegardés.

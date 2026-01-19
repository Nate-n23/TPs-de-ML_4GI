# TPs de Machine Learning - 4GI

Ce dépôt contient les travaux pratiques (TPs) réalisés dans le cadre du module de Machine Learning. Il couvre le pipeline complet de Machine Learning, de l'exploration des données à la mise en production (MLOps), en passant par la régression et le clustering.

## Contenu du Projet

Le projet est structuré en trois notebooks principaux :

*   **`TP1.ipynb` - Pipeline Machine Learning & Data Processing** :
    *   Introduction au pipeline ML.
    *   Collecte, description et résumé des données.
    *   Nettoyage et préparation des données (Data Wrangling).
    *   Visualisation des données (Data Visualization).

*   **`TP2.ipynb` - Régression & MLOps** :
    *   Régression Linéaire (OLS, Descente de Gradient).
    *   Compromis Biais-Variance.
    *   Régularisation (Ridge, Lasso) et optimisation des hyperparamètres.
    *   **MLOps** : Tracking des expériences avec **MLflow**, packaging de modèle, et containerisation avec **Docker**.

*   **`TP3.ipynb` - Clustering & Analyse Non-Supervisée** :
    *   Algorithmes de clustering : **K-Means** et **GMM (Gaussian Mixture Models)**.
    *   Optimisation : Méthode du Coude (Elbow Method), Coefficient de Silhouette.
    *   Cas d'usage : Segmentation client.
    *   Intégration MLOps pour le clustering.

## Prérequis

*   **Python 3.9+**
*   **pip** (gestionnaire de paquets Python)

## Installation

Pour exécuter les notebooks sur votre machine locale, suivez ces étapes :

1.  **Cloner le dépôt :**

    ```bash
    git clone <URL_DU_DEPOT>
    cd <NOM_DU_DOSSIER>
    ```

2.  **Créer un environnement virtuel (recommandé) :**

    ```bash
    # Création de l'environnement
    python -m venv venv

    # Activation de l'environnement
    # Sur Linux/MacOS :
    source venv/bin/activate
    # Sur Windows :
    # venv\Scripts\activate
    ```

3.  **Installer les dépendances :**

    ```bash
    pip install -r requirements.txt
    ```

## Utilisation

Une fois les dépendances installées et l'environnement activé, vous pouvez lancer Jupyter Notebook pour explorer les TPs :

```bash
jupyter notebook
```

Cela ouvrira une interface dans votre navigateur où vous pourrez cliquer sur `TP1.ipynb`, `TP2.ipynb` ou `TP3.ipynb` pour les exécuter.

### Docker (Optionnel pour TP2/TP3)

Le projet contient un `Dockerfile` (référencé dans TP2) pour containeriser l'application. Pour construire et lancer l'image Docker :

```bash
# Construire l'image (assurez-vous d'être dans le dossier contenant le Dockerfile)
docker build -t tp-ml-app .

# Lancer le conteneur
docker run -p 5000:5000 tp-ml-app
```

## Technologies Utilisées

*   **Langage** : Python
*   **Bibliothèques Principales** :
    *   `numpy`, `pandas` : Manipulation de données.
    *   `matplotlib`, `seaborn` : Visualisation.
    *   `scikit-learn` : Modélisation (Régression, Clustering).
    *   `mlflow` : Tracking d'expériences et gestion du cycle de vie ML.
    *   `joblib` : Sérialisation des modèles.

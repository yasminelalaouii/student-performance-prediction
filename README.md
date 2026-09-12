# Prédiction de la réussite des étudiants

Ce projet explore les facteurs qui influencent les résultats scolaires des étudiants (heures d'étude, présence, sommeil, soutien parental, etc.) et compare plusieurs modèles de machine learning pour prédire si un étudiant obtiendra un score d'examen au-dessus ou en dessous de la médiane.

## Données

Le dataset utilisé est **Student Performance Factors** disponible sur Kaggle :
 https://www.kaggle.com/datasets/lainguyn123/student-performance-factors/data

Pour reproduire ce projet :
1. Télécharger le fichier `data.csv` depuis le lien Kaggle ci-dessus (nécessite un compte Kaggle gratuit).
2. Placer `data.csv` dans le même dossier que le notebook.

## Contenu du notebook

- **Analyse exploratoire des données (EDA)** : distributions, valeurs manquantes, corrélations, visualisations (histogrammes, boxplots, heatmap, pairplot).
- **Prétraitement** : encodage des variables catégorielles avec `OneHotEncoder`.
- **Modèles de classification** (prédire si le score est au-dessus/en-dessous de la médiane) :
  - Arbre de décision (avec comparaison des critères gini / entropy / log_loss et visualisation de l'arbre)
  - SVM (noyau linéaire et RBF)
  - Naive Bayes
  - Régression logistique
- **Clustering non supervisé** :
  - K-Means (méthode du coude pour choisir le nombre de clusters)
  - Clustering hiérarchique (dendrogramme)
  - DBSCAN
  - Visualisation via PCA (réduction à 2 dimensions)

## Installation

```bash
pip install -r requirements.txt
```

## Utilisation

Ouvrir le notebook avec Jupyter :

```bash
jupyter notebook student_performance_prediction.ipynb
```

et exécuter les cellules dans l'ordre.

## Technologies

Python, pandas, numpy, matplotlib, seaborn, scikit-learn, dtreeviz

# Student Performance Prediction

This project explores the factors that influence students' academic outcomes (study hours, attendance, sleep, parental support, etc.) and compares several machine learning models to predict whether a student's exam score will fall above or below the median.

## Data

The dataset used is **Student Performance Factors**, available on Kaggle:
https://www.kaggle.com/datasets/lainguyn123/student-performance-factors/data

To reproduce this project:
1. Download the `data.csv` file from the Kaggle link above (requires a free Kaggle account).
2. Place `data.csv` in the same folder as the notebook.

## Notebook Contents

- **Exploratory Data Analysis (EDA)**: distributions, missing values, correlations, visualizations (histograms, boxplots, heatmap, pairplot).
- **Preprocessing**: categorical variable encoding with `OneHotEncoder`.
- **Classification models** (predicting whether the score is above/below the median):
  - Decision Tree (comparing gini / entropy / log_loss criteria, with tree visualization)
  - SVM (linear and RBF kernels)
  - Naive Bayes
  - Logistic Regression
- **Unsupervised clustering**:
  - K-Means (elbow method to choose the number of clusters)
  - Hierarchical clustering (dendrogram)
  - DBSCAN
  - Visualization via PCA (dimensionality reduction to 2D)

## Installation

```bash
pip install -r requirements.txt
```

## Usage

Open the notebook with Jupyter:

```bash
jupyter notebook student_performance_prediction.ipynb
```

and run the cells in order.

## Technologies

Python, pandas, numpy, matplotlib, seaborn, scikit-learn, dtreeviz

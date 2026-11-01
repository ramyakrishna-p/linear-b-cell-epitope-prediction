# Linear B-Cell Epitope Prediction

**Machine Learning / Data Mining - Ramya Krishna Parimi (Student ID: 250135187), CS4850 Data Mining, Aston University**

Machine learning pipeline for predicting linear B-cell epitopes in protein sequences from a human pathogen, using ESM-2 protein embeddings plus traditional bioinformatics features.

## Dataset and approach
- High-dimensional dataset: ~50,000 rows, 1,651 columns (ESM-2 embeddings and bioinformatics features)
- Exploratory data analysis, feature scaling, class imbalance handling and feature reduction
- Group-aware cross-validation using the Info_group variable to avoid data leakage
- Models compared included Logistic Regression, Random Forest and gradient boosting (XGBoost / LightGBM)
- Primary metric: Balanced Accuracy (appropriate for the observed class imbalance)

## Results (from the notebook's own outputs)
- Best model: Logistic Regression, tuned C=0.1, penalty l2, solver liblinear
- Cross-validation Balanced Accuracy: 0.7124
- Held-out test set (10,000 rows): Balanced Accuracy 0.7812, ROC-AUC 0.8503, Accuracy 0.8378, weighted F1 0.8989

## Files
- `250135187_Code.ipynb` - full original notebook with outputs

All results above are taken from this notebook, which is Ramya's own coursework.

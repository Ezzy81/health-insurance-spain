# Health Insurance Portfolio - Analyse et Machine Learning

## Dataset
- Source : Mendeley Data (Espagne)
- 228 711 lignes x 42 colonnes
- Periode : 2017-2019

## Objectifs
- Analyser la rentabilite du portefeuille
- Predire le cout des sinistres
- Classifier les assures rentables
- Predire les resiliations (churn)

## Stack technique
Python, Pandas, Scikit-learn, XGBoost, SHAP, Matplotlib, Seaborn, Power BI

## Resultats ML
| Modele | Type | Resultat |
|--------|------|----------|
| Random Forest | Regression cout sinistres | MAE 389 euros, R2 0.37 |
| XGBoost | Classification rentabilite | Accuracy 89%, F1 0.94 |
| XGBoost | Prediction churn | Recall 0.78 |

## Points cles
- Dataset rare espagnol — pas un dataset Kaggle classique
- Data leakage detecte et corrige
- SHAP utilise pour expliquer les predictions
- n_medical_services est la variable la plus predictive

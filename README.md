# 🏥 Portefeuille Assurance Santé — Analyse & Machine Learning

> Analyse complète d’un portefeuille d’assurance santé espagnol (2017-2019) avec modèles ML et dashboard Power BI interactif.

-----

## 📊 Dashboard Power BI

### Vue Générale

![Vue Générale](dashboard/Vue%20Générale.png)

### Segments à Risque

![Segments à Risque](dashboard/Segments%20à%20risque.png)

### Prédictions ML

![Prédictions ML](dashboard/Prédictions%20ML.png)

-----

## 📁 Jeu de données

|Caractéristique|Détail                 |
|---------------|-----------------------|
|*Source*     |Mendeley Data (Espagne)|
|*Lignes*     |228 711                |
|*Colonnes*   |42                     |
|*Période*    |2017 - 2019            |


> Dataset rare espagnol — ce n’est pas un dataset Kaggle classique.

-----

## 🎯 Objectifs

- Analyser la rentabilité du portefeuille d’assurance santé
- Prédire le coût des sinistres par assuré
- Classifier les assurés selon leur rentabilité
- Prédire les résiliations (churn)

-----

## 🛠️ Stack technique

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189AB4?style=flat)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)

Python · Pandas · Scikit-learn · XGBoost · SHAP · Matplotlib · Seaborn · Power BI

-----

## 🤖 Résultats ML

|Modèle       |Type                      |Résultat                      |
|-------------|--------------------------|------------------------------|
|Random Forest|Régression coût sinistres |MAE : 389€ · R² : 0.37        |
|XGBoost      |Classification rentabilité|Accuracy : 89% · F1 : 0.94    |
|XGBoost      |Prédiction churn          |Recall : 0.78 · Accuracy : 80%|

-----

## 💡 Points clés

- 🇪🇸 *Dataset rare espagnol* — pas un dataset Kaggle classique
- 🔍 *Data leakage détecté et corrigé* pendant la phase de modélisation
- 🧠 *SHAP utilisé* pour expliquer les prédictions modèle par modèle
- 📌 *n_medical_services* est la variable la plus prédictive du coût sinistres

-----

## 📂 Structure du projet


health-insurance-spain/
├── dashboard/                  # Screenshots Power BI
│   ├── Vue Générale.png
│   ├── Segments à risque.png
│   └── Prédictions ML.png
├── data/
│   ├── raw/                    # Données brutes originales
│   ├── processed/              # Données nettoyées
│   └── exports/                # Export pour Power BI
├── notebooks/
│   └── analyse_propre.ipynb    # Notebook principal
├── reports/figures/            # Graphiques générés
├── src/                        # Modèles ML sauvegardés
│   ├── model_regression.pkl
│   ├── model_classification.pkl
│   └── model_churn.pkl
├── .gitignore
├── requirements.txt
└── README.md


-----

## 🚀 Installation

bash
# Cloner le repo
git clone https://github.com/Ezzy81/health-insurance-spain.git
cd health-insurance-spain

# Installer les dépendances
pip install -r requirements.txt

# Lancer le notebook
jupyter notebook notebooks/analyse_propre.ipynb


-----

## 👤 Auteur

*Ezzy81* — [GitHub](https://github.com/Ezzy81)
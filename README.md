# 🔍 Détection de Fraude - Classificateur Arbre de Décision

Ce projet implémente un pipeline complet de détection de fraude utilisant un classificateur d'arbre de décision (DecisionTreeClassifier) avec optimisation des hyperparamètres via GridSearchCV.

## 📋 Description

Le projet couvre l'ensemble du processus de modélisation pour la détection de transactions frauduleuses :
- **Analyse Exploratoire des Données (EDA)** : Exploration des données, visualisation des distributions et corrélations.
- **Ingénierie des Fonctionnalités** : Traitement des valeurs manquantes, création de nouvelles variables et encodage des variables catégorielles.
- **Modélisation** : Entraînement d'un modèle DecisionTreeClassifier avec recherche d'hyperparamètres optimaux.
- **Évaluation** : Analyse des performances avec métriques classiques (accuracy, precision, recall, F1-score, ROC-AUC).
- **Soumission** : Génération d'un fichier de prédictions pour soumission.

## 🛠️ Prérequis

- Python 3.7+
- Bibliothèques : pandas, numpy, matplotlib, seaborn, scikit-learn

## 📦 Installation

1. Clonez ce dépôt :
   ```bash
   git clone https://github.com/nekemanuella2-web/TP-Decision-Tree.git
   cd votre-repo
   ```

2. Installez les dépendances :
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

## 🚀 Utilisation

1. **Préparation des données** : Assurez-vous que le fichier `Fraud Detection Dataset.csv` est dans le répertoire racine.

2. **Exécution du notebook** : Ouvrez et exécutez le notebook `decision_tree.ipynb` dans Jupyter Notebook ou VS Code.

3. **Génération des résultats** : Le notebook génère automatiquement :
   - `submission_predictions.csv` : Fichier de prédictions
   - `model_report.txt` : Rapport détaillé du modèle

## 📁 Structure du Projet

- `decision_tree.ipynb` : Notebook principal avec le pipeline complet
- `Fraud Detection Dataset.csv` : Dataset des transactions
- `model_report.txt` : Rapport généré du modèle
- `submission_predictions.csv` : Prédictions générées

## 📊 Résultats

### Métriques de Performance (Test Set)
- **Accuracy** : 0.5166
- **Precision** : 0.0426
- **Recall** : 0.4104
- **F1-Score** : 0.0771
- **ROC-AUC** : 0.4587

### Meilleurs Hyperparamètres
- class_weight: balanced
- criterion: gini
- max_depth: 5
- min_samples_leaf: 1
- min_samples_split: 2

### Top 5 Fonctionnalités Importantes
1. Transaction_Frequency_Ratio (0.2302)
2. Amount_per_Account_Age (0.1551)
3. Time_of_Transaction (0.1248)
4. Payment_Method_encoded (0.1234)
5. Transaction_Amount (0.0974)

### Dataset
- **Échantillons totaux** : 51,000
- **Fonctionnalités** : 17
- **Taux de fraude** : 4.92%

## 🤝 Contribution

Les contributions sont les bienvenues ! Veuillez ouvrir une issue ou soumettre une pull request.


## 👤 Auteur

[NEKE Manuella Yayra Adjogan] - [nekemanuella2@gmail.com]

---

*Projet réalisé dans le cadre d'un devoir sur la détection de fraude.*
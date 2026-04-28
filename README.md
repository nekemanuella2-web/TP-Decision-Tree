# Detection de Fraude - Devoir Decision Tree

Ce depot contient un devoir simple de data mining / machine learning autour de la detection de fraude.
Le travail se concentre sur trois points :
- une EDA courte pour comprendre les donnees ;
- un peu de feature engineering ;
- un modele de base `DecisionTreeClassifier` avec une recherche simple d'hyperparametres.

## Contenu

- `decision_tree.ipynb` : notebook principal a rendre
- `Fraud Detection Dataset.csv` : jeu de donnees
- `images/` : graphiques generes pendant l'analyse et l'evaluation

## Etapes du devoir

1. Charger et decrire rapidement le dataset
2. Faire une EDA legere avec quelques graphiques utiles
3. Traiter les valeurs manquantes
4. Creer quelques variables simples
5. Entrainer un arbre de decision
6. Chercher de meilleurs hyperparametres avec `GridSearchCV`
7. Evaluer le modele avec les metriques principales

## Lancement

Installez les bibliotheques si besoin :

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Puis ouvrez `decision_tree.ipynb` dans Jupyter ou VS Code.

## Remarque

Le but ici n'est pas de construire une solution de competition, mais de montrer une demarche claire et propre de base en EDA, feature engineering et modelisation.
Le notebook se termine aussi par quelques remarques simples sur les donnees, le modele et les resultats, pour garder une conclusion de devoir claire et complete.

# Detection de Fraude - Devoir Decision Tree

Ce depot contient un devoir simple de data mining / machine learning autour de la detection de fraude.
Le travail se concentre sur trois points :
- une EDA courte pour comprendre les donnees ;
- un peu de feature engineering ;
- un modele de base `DecisionTreeClassifier` avec une recherche simple d'hyperparametres.

## Contenu

- `decision_tree.ipynb` : notebook principal a rendre
- `Fraud Detection Dataset.csv` : jeu de donnees
- `images/` : graphiques generes pendant l'analyse et l'evaluation, y compris la comparaison baseline vs optimisation

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

Le notebook se termine aussi par quelques remarques simples sur les donnees, le modele et les resultats, pour garder une conclusion de devoir claire et complete

## Conclusion

Le jeu de donnees est desequilibre, avec peu de fraudes par rapport aux transactions normales, ce qui rend la detection plus difficile.

Les resultats restent limites, et l'AUC est faible, ce qui montre que le modele distingue encore mal les transactions frauduleuses des transactions normales. Cela semble venir a la fois du jeu de donnees, qui est desequilibre et peu separable, et du fait que le modele utilise reste simple.

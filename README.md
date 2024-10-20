## House price prediction 

### Description du Projet

Ce projet vise à prédire les prix de loyer des maisons en fonction de plusieurs caractéristiques. Les modèles de prédiction utilisés sont la forêt aléatoire (RandomForest) et la régression linéaire (LinearRegression). Les caractéristiques utilisées pour l'entraînement des modèles incluent :

    SquareFeet : Superficie en pieds carrés
    Bedrooms : Nombre de chambres
    Bathrooms : Nombre de salles de bain
    YearBuilt : Année de construction
    Price : Prix de loyer (variable cible)
    Rural : Indicateur binaire pour les zones rurales
    Suburb : Indicateur binaire pour les banlieues
    Urban : Indicateur binaire pour les zones urbaines
    bedrooms_ratio : Ratio des chambres

### Prétraitement des Données

Le dataset initial comprenait une colonne textuelle nommée Neighboorhoud, qui indiquait le type de quartier (Rural, Suburb, Urban). Pour pouvoir utiliser cette colonne dans nos modèles de machine learning, nous avons appliqué la méthode get_dummies pour convertir cette colonne textuelle en colonnes numériques binaires.

### Modèles Utilisés

Deux modèles principaux ont été utilisés pour prédire les prix des loyers :

    RandomForest
        Avantages : Peut gérer des relations non linéaires, robuste aux données bruitées, et offre une bonne précision.
        Inconvénients : Peut être lent à l'entraînement et à la prédiction sur de grandes datasets, nécessite une optimisation des hyperparamètres.

    LinearRegression
        Avantages : Simplicité et rapidité, facile à interpréter, bonne performance sur les données linéaires.
        Inconvénients : Performances limitées sur des relations non linéaires, sensible aux outliers.


La dataset utilisé se trouve ici : [https://www.kaggle.com/datasets/muhammadbinimran/housing-price-prediction-data]
cette dataset contient les colonnes suivantes : SquareFeet, Bedrooms, Bathrooms, YearBuilt,Price et Neighboorhoud

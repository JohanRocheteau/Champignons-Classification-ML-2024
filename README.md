# Projet Formation Continue : Classification des Champignons
![Logo](photos/Morilles.jpg)


## Mise en situation :
- **But :** Catégoriser les champignons en fonction de leur comestibilité, que ce soit à travers leur description (mesures ou textes) ou leur photo.
- **Jeux de données :** [Guides des Champignons](https://www.guidedeschampignons.com/)
- **Information : ** Toutes les photos sont issues du site : "https://www.guidedeschampignons.com/"


## Réalisations :
- **Librairies principales :** Selenium, PIL, NLTK, Spacy, Pymongo, divers modèles de ML, VGG16, GridSearchCV, BayesSearchCV
   
- **Etapes réalisées : **
    - **Scrapping des données :**
	- Ouvertures des fichiers
	- Création/modifications des variables (par calculs, dummisations, factorisation) grâce au code de Kaggle
	- Merge des fichiers 
	- Création de fichiers moins lourds pour GitHub (25Mo max)
	- Récupération des nouveaux clients pour l'application

    - **Etude du déséquilibre des données et choix d'un modèle de Machine Learning :**
	- Utilisation de MLFlow pour le suivi et la comparaison des runs
	- Création de deux métriques pour ajouter du poids aux faux négatifs
	- **Comparaison de diverses façons de gérer le déséquilibre des données :** SMOTE, Class_Weight, Undersampling, Oversampling

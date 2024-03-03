# Projet Formation Continue : Classification des Champignons
![Logo](photos/Morilles.jpg)


## Mise en situation :
- **But :** Catégoriser les champignons en fonction de leur comestibilité, que ce soit à travers leur description (mesures ou textes) ou leur photo.
- **Problématique :** Ne trouvant pas de base de données Open Source sur les champignons, j'ai du aller chercher les données sur internet via scraping. 
- **Jeux de données :** [Guides des Champignons](https://www.guidedeschampignons.com/)
- **Information :** Toutes les photos sont la propriété du site le guide des champignons.


## Réalisations :
- **Librairies principales :** Selenium, PIL, NLTK, Spacy, Pymongo, divers modèles de ML, VGG16, GridSearchCV, BayesSearchCV
   
- **Etapes réalisées : **
    - **Scrapping des données :**
	- **Objectif :** Passer de champignon en champignon et récupérer le maximum d'informations (textes et photo).
      	![Logo](photos/LesChampignons.png)
          
      	![Logo](photos/Champignon.png)
	- **Stockage :**
 		- Les données sont stockées sous format DataFrame :
     		![Logo](photos/DatatFrameInitiale.png)
   		- Les photos sont stockées sur mon ordinateur.

    - **Etude du déséquilibre des données et choix d'un modèle de Machine Learning :**
	- Utilisation de MLFlow pour le suivi et la comparaison des runs
	- Création de deux métriques pour ajouter du poids aux faux négatifs
	- **Comparaison de diverses façons de gérer le déséquilibre des données :** SMOTE, Class_Weight, Undersampling, Oversampling

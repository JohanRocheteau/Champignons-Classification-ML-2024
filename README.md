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
	- **Objectif :** Passer de champignon en champignon et scraper le maximum d'informations (textes et photo).
      	![Logo](photos/LesChampignons.png)
          
      	![Logo](photos/Champignon.png)
	- **Stockage :**
 		- Les données sont stockées sous format DataFrame :
     		![Logo](photos/DataFrameInitiale.png)
   		- Les photos sont stockées sur mon ordinateur.

    - **Analyse et Nettoyage des données :**
	- Extraction des données chiffrées (tailles chapeaux et pieds).
 	- Extraction de la saisonnalité des champignons.
  	- Pool des diverses informations textuelles et extractions des mots pertinents via NLP.
  	- Divers graphiques et visuels :
  	  
  	- Création de deux catégories : Comestible et Non Comestible
  	- Stockage des données dans une DataFrame Nettoyée et exportée en CSV/Excel ou sur MongoDB Compass.

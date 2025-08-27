# Champignons-Classification-ML-2024

![Illustration](photos/Morilles.jpg)

Projet de formation continue réalisé en 2024 visant à classifier des champignons selon leur comestibilité, en combinant du scraping web, du traitement de texte (NLP), de l’analyse d’images, et du machine learning supervisé et non supervisé.

## Objectifs

- Construire un jeu de données sur les champignons à partir de sources en ligne
- Classifier les champignons comme comestibles ou non comestibles
- Tester des approches d’apprentissage machine sur des données textuelles et visuelles
- Identifier les limites liées au volume et à la qualité des données

## Données

- **Source** : [Le guide des champignons](https://www.guidedeschampignons.com/)
- **Format** :  
  - Texte descriptif (caractéristiques, saisonnalité)  
  - Images locales  
  - Stockage : DataFrame, CSV/Excel, ou MongoDB Compass  
- **Droits** : Les images sont la propriété du site cité ci-dessus.

## Méthodologie

### 1. Scraping et extraction des données

- Navigation automatisée avec Selenium pour collecter les informations de chaque champignon.
- Téléchargement des photos associées.

![Scraping](photos/LesChampignons.png)
![Exemple](photos/Champignon.png)
![Aperçu des données](photos/DataFrameInitiale.png)

### 2. Préparation et exploration des données

- Nettoyage des descriptions textuelles
- Extraction de variables structurées (taille du chapeau, saisonnalité…)
- NLP : sélection des mots-clés pertinents
- Visualisation : word cloud, top mots, graphiques, tableaux croisés

![Graphiques](photos/Graphiques.png)
![Graphique 2](photos/Graphique2.png)
![Tableau croisé](photos/TableauCroisé.png)
![Top mots](photos/TopTen.png)
![Word cloud](photos/WordCloud.png)

### 3. Classification supervisée et non supervisée

#### Non supervisé
- Test du clustering avec **KMeans**
- Résultat très faible (ARI ≈ 0)

![KMeans](photos/ClassificationNonSupervisée.png)

#### Supervisé
- Modèles avec données textuelles (TFIDF) et images (VGG16)
- Optimisation via **GridSearchCV** et **BayesSearchCV**
- Tests avec et sans augmentation de données

![Résultat 1](photos/Resultat1.png)
![Résultat 2](photos/Resultat2.png)
![Détourage](photos/PhotoDetouree.png)
![Résultat 3](photos/Resultat3.png)

## Résultats

- Faible performance globale, notamment due au manque de données
- Présence d’overfitting sur plusieurs modèles testés
- Données images peu discriminantes avec les approches utilisées
- Modèles non adaptés à une mise en production en l’état

## Limites et perspectives

- Jeu de données trop limité pour entraîner des modèles robustes
- Tentative de contact avec **MycoDB** pour enrichir les données (sans réponse)
- Idée d’un score de sécurité pour éviter les faux positifs "comestibles"
- Une application **Streamlit** pourrait être envisagée si un dataset plus fiable est obtenu

## Technologies utilisées

- **Langage** : Python
- **Librairies** : Selenium, PIL, NLTK, Spacy, Pymongo, VGG16, scikit-learn, GridSearchCV, BayesSearchCV
- **Environnement** : Jupyter Notebook

## Contact

Projet réalisé en 2024 dans le cadre d’une formation continue en Data Science.  
Pour toute question ou suggestion :

- **Email** : [johan.rocheteau@hotmail.fr](mailto:johan.rocheteau@hotmail.fr)  
- **LinkedIn** : [linkedin.com/in/johan-rocheteau](https://www.linkedin.com/in/johan-rocheteau)

# Projet Personnel : Classification des Champignons

![Logo](PhotosReadme/LogoChampignons.png)  

## **📌 Contexte et Objectif**

**But :** Classifier les champignons en fonction de leur comestibilité en utilisant un modèle de machine learning.  
**Problématique :** Identifier si un champignon est comestible ou non à partir de caractéristiques numériques et d'images.

### 🔍 **Problématiques étudiées :**
- Comment classifier les champignons en comestible/non comestible ?
- Quels sont les modèles de machine learning les plus efficaces pour cette classification ?
- Quelle est l'importance des données d'images et de caractéristiques physiques pour cette tâche ?

📂 **Jeux de données :**
- 📊 Source : [UCI Mushroom Data Set](https://archive.ics.uci.edu/ml/datasets/Mushroom)
- 📥 [Téléchargement du dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00360/)

---

## **🚀 Réalisations et Méthodologie**

### 🔹 **1️⃣ Préparation des données**
- Chargement et exploration des données depuis le fichier CSV.
- Nettoyage des données et transformation des variables catégorielles en format numérique.
- Identification des valeurs manquantes et traitement des doublons.

### 🔹 **2️⃣ Modélisation et Machine Learning**
- Sélection des caractéristiques pertinentes pour la classification.
- Utilisation des modèles de machine learning tels que **Random Forest**, **SVM** et **KNN** pour classer les champignons.
- Optimisation des hyperparamètres à l’aide de **GridSearchCV** et **BayesSearchCV**.

### 🔹 **3️⃣ Analyse et Visualisation des résultats**
- Evaluation des performances des modèles avec des métriques comme **accuracy**, **recall**, **precision**.
- Création de graphiques pour illustrer la comparaison des modèles.
  
📊 **Exemples de visualisations :**

![Graphique 1](PhotosReadme/Graph1.png)  
![Graphique 2](PhotosReadme/Graph2.png)  

---

## **📈 Résultats et Insights Clés**

### 🔎 **Conclusions de l'analyse :**
✔ Les **Random Forests** ont montré les meilleures performances pour la classification.  
✔ L'importance des caractéristiques physiques des champignons a été démontrée dans les résultats.  
✔ Des améliorations peuvent être apportées avec plus de données d'images et un affinement des hyperparamètres.

### 📌 **Recommandations pour de futurs travaux :**
1️⃣ Intégrer des données d’images pour améliorer la performance du modèle.  
2️⃣ Tester de nouveaux modèles de deep learning pour l’analyse d’images (CNN).  
3️⃣ Collecter davantage de données pour améliorer la généralisation du modèle.

---

## **🛠️ Technologies et Outils Utilisés**

- **Langage** : Python 🐍  
- **Librairies** : Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Environnement** : Jupyter Notebook  
- **Méthodes utilisées** : Classification supervisée, Evaluation de modèles, Optimisation des hyperparamètres  

---

## **📬 Contact et Feedback**

💡 Ce projet a été réalisé dans le cadre d’une **formation personnelle en Data Science**. N’hésitez pas à **laisser vos suggestions** ou à me **contacter** pour en discuter !

📩 **Contact :**  
📧 [johan.rocheteau@hotmail.fr](mailto:johan.rocheteau@hotmail.fr)  
🔗 [LinkedIn](https://www.linkedin.com/in/johan-rocheteau)

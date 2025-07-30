# 🛡️ Microsoft Malware Prediction

Ce projet a pour objectif de prédire la probabilité qu’un ordinateur sous Windows soit infecté par un logiciel malveillant (malware), à partir de ses caractéristiques système. Le dataset utilisé est dérivé de la compétition Kaggle [Microsoft Malware Prediction](https://www.kaggle.com/competitions/microsoft-malware-prediction).

## 📁 Description du projet

Nous avons exploré des techniques d’**apprentissage supervisé** et **non supervisé** pour :

- Comprendre les facteurs contribuant à l’infection
- Créer un modèle de prédiction fiable
- Identifier des groupes de machines similaires via le clustering

---

## 🧪 Partie 1 : Apprentissage Supervisé

### 🔍 Analyse exploratoire
- Chargement des données
- Informations générales (`df.info()`, `df.describe()`)
- Rapport de profilage via **Pandas Profiling** pour détecter :
  - Valeurs manquantes
  - Corrélations
  - Distributions

### 🧹 Prétraitement
- Suppression des doublons
- Traitement des valeurs manquantes
- Traitement des valeurs aberrantes (IQR)
- Encodage des variables catégorielles (OneHotEncoder)
- Normalisation des données si nécessaire

### 🌲 Modélisation
- Modèle principal : **Arbre de Décision (Decision Tree Classifier)**
- Optimisation des hyperparamètres (max_depth, min_samples_split, etc.)
- Évaluation :
  - **Matrice de confusion**
  - **Courbe ROC / AUC**
  - **Accuracy**, **F1-score**, **Recall**, **Precision**

---

## 🤖 Partie 2 : Apprentissage Non Supervisé

### 🎯 Objectif
Identifier des groupes similaires de machines sans utiliser la variable cible.

### 📊 Clustering
- Algorithme : **K-Means**
- Suppression de la variable cible
- Détermination du nombre optimal de clusters via la **méthode du coude (elbow method)**
- Visualisation des clusters
- Interprétation des résultats (facteurs principaux de regroupement)

---

## 🧰 Outils et bibliothèques utilisés

- Python 3.x
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Pandas Profiling
- Jupyter Notebook

---

## 📌 Résultats clés

- Modèle de classification performant avec un bon équilibre entre précision et rappel
- Insights intéressants sur les variables les plus corrélées aux infections
- Segmentation efficace via le clustering, ouvrant la voie à des stratégies de prévention ciblées

---

## 📎 Ressources

- 📄 Dataset original : [Kaggle Microsoft Malware Prediction](https://www.kaggle.com/competitions/microsoft-malware-prediction)
- 📸 Diagramme des variables : ![Diagramme des colonnes](https://i.imgur.com/hv2Ynyn.jpg)

---

## 📫 Contact: cheikhniang159@gmail.com

Pour toute question ou collaboration, n'hésitez pas à me contacter sur [LinkedIn](https://www.linkedin.com) ou via mail.

---


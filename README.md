## Aperçu de l'entreprise

![Aperçu du site web](images/DS_projet6.PNG)

## 📌 Contexte professionnel

En tant que **Data Scientist** chez **Place de Marché**, j’ai été missionné pour étudier la faisabilité de l’automatisation de la **catégorisation des articles** à partir de leurs **descriptions textuelles** et **images**, afin de remplacer un processus manuel chronophage et peu fiable.

Le projet est structuré en deux volets :
1. Une **étude de faisabilité** utilisant des techniques de NLP et de vision par ordinateur pour explorer différentes méthodes de classification.
2. Une phase de **mise en œuvre opérationnelle** incluant la classification supervisée par CNN et l’intégration d’une API pour l’extraction automatisée de données produit.

---

## 🎯 Objectifs de la mission

- Automatiser la **classification des articles** en catégories à partir de données textuelles et visuelles
- Comparer différentes **méthodes d’encodage et d’extraction de features**
- Implémenter un **modèle supervisé d’image classification**
- Tester une **API externe** pour enrichir les données produits
- Fournir une **présentation métier** des résultats obtenus

---

## 🧩 Étapes de réalisation

### 📘 Première mission : étude de faisabilité

#### 1. NLP – Méthodes basiques

- Prétraitement des textes (stopwords, lemmatisation)
- Encodage avec **Bag of Words** et **TF-IDF**
- Réduction de dimension (**PCA**, **t-SNE**)
- Visualisation des clusters par catégorie

#### 2. NLP – Méthodes avancées

- Embeddings avec **Word2Vec**, **BERT**, **USE**
- Réduction de dimension et projection
- Comparaison de la cohérence des clusters avec les catégories réelles

#### 3. Computer Vision – Méthodes basiques

- Prétraitement d’image : niveaux de gris, contraste, etc.
- Extraction de features avec **SIFT**, **ORB** (OpenCV)
- Clustering et réduction de dimension pour analyse visuelle

#### 4. Computer Vision – Méthodes avancées

- **Transfer Learning** avec **ResNet**, **VGG**
- Extraction des embeddings visuels
- Analyse de la pertinence des clusters formés par catégorie

---

### 📗 Deuxième mission : mise en œuvre opérationnelle

#### 1. Classification supervisée d’images

- Modèle de **CNN Transfer Learning**
- **Data augmentation** pour généralisation
- Évaluation par **accuracy** et **F1-score**

#### 2. Intégration API produit

- Appels API pour requêter des produits "champagne"
- Récupération des champs : foodId, label, category, etc.
- Enregistrement dans un fichier **CSV**

#### 3. Présentation finale

- Diaporama structuré : problématique, méthodologie, résultats
- Comparaison des méthodes NLP et Vision
- Recommandations stratégiques pour l’intégration future

---

## 📂 Livrables

- **Notebook NLP Basique et Avancé**
- **Notebook Computer Vision Basique et Avancé**
- **Notebook CNN Classification Supervisée**
- **Script d’intégration API**
- **Présentation finale PDF (30 slides max)**

---

## 🛠️ Outils et technologies

- **Python** (pandas, scikit-learn, TensorFlow, Keras)
- **OpenCV** pour l’extraction d’attributs visuels
- **NLP** : TF-IDF, Word2Vec, BERT, USE
- **Modèles visuels pré-entraînés** : ResNet, VGG
- **API Requests** pour l’appel d’API
- Visualisation avec **matplotlib**, **seaborn**, **PCA**, **t-SNE**

---

## ✅ Résultats et impact

- Comparaison rigoureuse entre méthodes basiques et avancées en NLP & Computer Vision
- Prototype de modèle supervisé prêt à intégrer une **chaîne de traitement e-commerce**
- Méthodologie reproductible pour enrichir la base de données produits
- Recommandations concrètes pour automatiser la catégorisation produit

---

## 🔍 Aperçu

> Ce projet démontre mes compétences en **NLP, Computer Vision, intégration API et classification supervisée**, dans un cas d’usage complet de **Data Science appliquée à l’e-commerce**.

---

*Projet réalisé dans un cadre professionnel simulé, avec des responsabilités comparables à celles d’un Data Scientist en startup tech e-commerce.*

# OPC_DATA_SCIENTIST_PROJET6
Classifiez automatiquement des biens de consommation


# Classification des Articles et Extraction de Données - Place de Marché

## Contexte

Je suis Data Scientist au sein de **"Place de Marché"**, une entreprise souhaitant lancer une marketplace e-commerce. Actuellement, la catégorisation des articles sur la plateforme est effectuée manuellement par les vendeurs, ce qui est inefficace et peu fiable. Mon rôle est d'explorer la faisabilité de l'automatisation de cette tâche en utilisant des descriptions textuelles et des images pour classifier les articles en différentes catégories. Par la suite, je mènerai également des tests sur l'intégration d'une API pour extraire des données de produits.

Ce projet est divisé en deux missions principales : 
1. Une étude de faisabilité pour l'automatisation de la classification des articles.
2. La mise en place d'une classification supervisée des images et l'intégration d'une API pour récupérer des données de produits spécifiques.

---

## Première Mission : Étude de Faisabilité pour la Classification Automatique

L’objectif est de démontrer la faisabilité d’un moteur de classification des articles en utilisant des approches basées sur le traitement de texte et d'image. L’étude couvre l’extraction de features, la réduction de dimension, et la segmentation des données en clusters pour identifier les catégories de produits.

### Étape 1 : Étude de faisabilité en utilisant des méthodes NLP basiques

- **Objectif** : Prétraiter les descriptions textuelles des articles et utiliser des méthodes basiques d'encodage pour évaluer la faisabilité de regrouper les articles par catégorie.
- **Détails** :
  - Prétraiter les textes : nettoyage, suppression des stopwords, lemmatisation, etc.
  - Utiliser des méthodes basiques d'encodage des textes : **Bag of Words**, **Tf-idf**.
  - Réduire la dimensionnalité à l’aide de **PCA** ou **t-SNE** et comparer les résultats avec les catégories réelles.
- **Livrable** : Un notebook montrant le prétraitement des textes et les résultats obtenus avec des méthodes d'encodage basiques.

### Étape 2 : Étude de faisabilité avec des méthodes NLP avancées

- **Objectif** : Utiliser des techniques d'embedding plus avancées pour voir si les résultats s'améliorent par rapport aux méthodes basiques.
- **Détails** :
  - Appliquer des techniques comme **Word2Vec**, **BERT**, **Universal Sentence Encoder (USE)**.
  - Réduire la dimension des embeddings et visualiser les résultats pour comparer avec les catégories réelles.
  - Comparer la performance des méthodes avancées avec celles des méthodes basiques.
- **Livrable** : Un notebook comparant les résultats obtenus avec des méthodes avancées d'embedding et leurs visualisations.

### Étape 3 : Étude de faisabilité en utilisant des techniques de traitement d'image basiques

- **Objectif** : Analyser les images des produits à l’aide de techniques de transformation et d'extraction de features d'image simples.
- **Détails** :
  - Appliquer des transformations d'image simples comme la conversion en niveaux de gris, le filtrage de bruit, et le contraste.
  - Utiliser des algorithmes d'extraction de features d'image comme **SIFT** ou **ORB**.
  - Réduire la dimension des features extraites et comparer les résultats avec les catégories réelles.
- **Livrable** : Un notebook détaillant les transformations d'images, l'extraction de features, et la réduction de dimension pour analyser la correspondance avec les catégories réelles.

### Étape 4 : Étude de faisabilité avec des techniques de traitement d'image avancées

- **Objectif** : Améliorer les résultats de classification en utilisant des modèles de **CNN Transfer Learning**.
- **Détails** :
  - Utiliser des modèles pré-entraînés comme **ResNet** ou **VGG** pour extraire des features d'image.
  - Comparer les résultats obtenus avec ceux des méthodes basiques d'extraction de features d'image.
  - Analyser la performance des modèles de **Transfer Learning** par rapport aux approches plus simples.
- **Livrable** : Un notebook comparant les résultats des méthodes de **CNN Transfer Learning** avec celles des méthodes d'extraction de features basiques.

---

## Deuxième Mission : Classification Supervisée et Test d'API

Après avoir prouvé la faisabilité de la classification automatique, je continue en mettant en place une classification supervisée pour les images des produits et un test d'API pour l'extraction de données de produits spécifiques.

### Étape 1 : Classification supervisée d'images via CNN Transfer Learning

- **Objectif** : Construire un modèle de classification supervisée pour prédire les catégories d'articles à partir d’images.
- **Détails** :
  - Utiliser un modèle de **CNN Transfer Learning** pour la classification des images.
  - Mettre en place une **data augmentation** pour améliorer la performance du modèle sur des petits ensembles de données.
  - Tester la performance du modèle avec des métriques comme l’accuracy et le **F1-score**.
- **Livrable** : Un notebook contenant le modèle de classification supervisée des images avec les résultats d’évaluation.

### Étape 2 : Test d'une API pour la collecte de données de produits

- **Objectif** : Intégrer une API pour récupérer des informations sur des produits à base de "champagne".
- **Détails** :
  - Utiliser l'API fournie pour récupérer les informations sur les produits en envoyant des requêtes via Python.
  - Extraire les données pertinentes (foodId, label, category, foodContentsLabel, image) et les enregistrer dans un fichier CSV.
  - Vérifier l’intégrité des données et gérer les éventuelles erreurs lors des requêtes API.
- **Livrable** : Un script ou notebook Python pour l’extraction des 10 premiers produits via l'API et génération du fichier CSV contenant les données.

### Étape 3 : Préparation de la présentation finale

- **Objectif** : Préparer une présentation structurée résumant l’ensemble des démarches, méthodes, et résultats obtenus.
- **Détails** :
  - Structurer la présentation autour des éléments suivants : problématique, jeu de données, prétraitements, extraction de features, résultats de classification, et test de l’API.
  - Justifier les choix méthodologiques, les résultats obtenus, et les recommandations.
  - Préparer une discussion autour des améliorations possibles et des axes futurs de recherche.
- **Livrable** : Un PDF de 30 slides maximum résumant les principales conclusions du projet.

---

## Détails Techniques

- **Fichiers** :
  - `Dataset des articles de Place de Marché` : Contient les images et descriptions des articles à classer.
  - **Notebook de Classification Textuelle** : Contient les prétraitements, l’extraction des features textuelles, et les visualisations des résultats de classification basique et avancée.
  - **Notebook de Classification d’Images** : Contient l’extraction des features d’image avec des méthodes basiques et avancées.
  - **Notebook de Classification Supervisée** : Contient le modèle de classification supervisée d'images.
  - **Script API** : Contient le code Python pour interagir avec l’API et extraire les données de produits à base de "champagne".

- **Outils Utilisés** :
  - **Python** (pandas, scikit-learn, TensorFlow, Keras) pour l'extraction des features, la classification, et l'API.
  - **OpenCV** pour le traitement d'images et l'extraction des features d'image avec SIFT/ORB.
  - **PCA**, **t-SNE** pour la réduction de dimension.
  - **API requests** pour l'extraction des données via API.

- **Compétences Utilisées** :
  - Traitement de texte et extraction des features avec Bag of Words, Tf-idf, et Word Embeddings.
  - Classification d'images avec des méthodes basiques et avancées.
  - Interaction avec une API pour l'extraction de données de produits.
  - Présentation des résultats et justifications des approches méthodologiques.

## Résumé

Ce projet consiste à développer une approche pour l’automatisation de la classification des articles sur une marketplace à partir de leurs images et descriptions textuelles. La première mission est dédiée à la faisabilité de la classification avec des méthodes basiques et avancées de traitement de texte et d’image. La seconde mission met en œuvre une classification supervisée à partir d’images et teste l’intégration d’une API pour extraire des données spécifiques de produits.

# Détection des fraudes bancaires par apprentissage automatique

## 1. Introduction
Ce projet porte sur la détection des fraudes bancaires à l'aide des techniques de machine learning. L'objectif est de développer un modèle capable d'identifier automatiquement les transactions frauduleuses à partir d'un ensemble de données provenant de Kaggle, accessible via le lien suivant : [Financial Transaction Fraud Dataset](https://www.kaggle.com/datasets/algozee/financial-transaction-fraud-dataset/code).

---

## 2. Présentation du jeu de données
L'ensemble de données contient des enregistrements de transactions bancaires comprenant des informations telles que :
* **Montant et temporalité :** Le montant de la transaction, la date et l'heure.
* **Comportement et contexte :** La catégorie du commerçant, la localisation du client et la fréquence des transactions.
* **Technologie :** Des informations sur l'appareil utilisé.
* **Cible :** Chaque enregistrement comprend une étiquette (*label*) indiquant si la transaction est normale ou frauduleuse.

Cet ensemble de données simule des comportements réalistes afin de permettre le développement et l'évaluation de modèles de détection des fraudes et de surveillance des risques dans le secteur financier.

---

## 3. Technologies utilisées
* **Langage :** Python 3.10+
* **Environnement :** Jupyter Notebook / Google Colab
* **Librairies Principales :**
  * Manipulations de données : `pandas`, `numpy`
  * Visualisation : `matplotlib`, `seaborn`
  * Machine Learning : `scikit-learn`, `xgboost`, `lightgbm` (à adapter selon vos modèles)

---

## 4. Installation
Pour exécuter ce projet localement, suivez les étapes suivantes :

1. **Cloner le dépôt :**
   ```bash
   git clone [https://github.com/taponjou/Fraud-Detection-Project.git](https://github.com/taponjou/Fraud-Detection-Project.git)
   cd Fraud-Detection-Project
   
---
## 5.  Structure du projet

---

## 6. Description des modèles
Dans le cadre de ce projet, plusieurs architectures d'apprentissage automatique ont été testées pour gérer le déséquilibre des classes (les transactions frauduleuses étant généralement très rares) :

**Régression Logistique : Modèle de référence (baseline).

**Random Forest / Extra Trees : Pour capturer les relations non linéaires.

**XGBoost / LightGBM : Algorithmes de boosting de gradient pour optimiser les performances de classification.

💡 Note : Des techniques de rééchantillonnage (comme SMOTE) ou d'ajustement des poids des classes ont été appliquées pour contrer le déséquilibre des données.

---

## 7. Résultats
Les performances sont évaluées principalement sur le Recall (pour minimiser les faux négatifs) et l'AUC-ROC.

---

## Auteur
. Taponjou - @taponjou

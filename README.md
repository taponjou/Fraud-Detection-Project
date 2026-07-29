# 🛡️ Détection de Fraudes Bancaires à l'aide du Machine Learning et du Deep Learning

## 📖 Présentation du projet

Ce projet a pour objectif de développer et de comparer plusieurs modèles de Machine Learning et de Deep Learning afin de détecter les transactions bancaires frauduleuses.

Le projet suit l'ensemble du cycle de vie d'un projet de Data Science, depuis l'exploration des données jusqu'à l'évaluation et la comparaison des modèles.

Les modèles développés comprennent :

- Régression Logistique
- Random Forest
- XGBoost
- Réseau de neurones Multi-Layer Perceptron (MLP) avec PyTorch

---

# 🎯 Objectifs

Les principaux objectifs de ce projet sont :

- Explorer et comprendre les données transactionnelles.
- Prétraiter les données pour les rendre exploitables.
- Traiter le déséquilibre des classes.
- Développer plusieurs modèles de classification.
- Optimiser un réseau de neurones MLP.
- Comparer les performances des différents modèles.
- Identifier le modèle offrant les meilleures performances pour la détection des fraudes.

---

# 📂 Structure du projet

```text
Fraud-Detection-Project/
│
├── clean_data 
│
├── notebooks/
│   ├── 01_Data_Exploration.ipynb
│   ├── 02_Data_Preprocessing.ipynb
│   ├── 03_Logistic_Regression.ipynb
│   ├── 04_Random_Forest.ipynb
│   ├── 05_XGBoost.ipynb
│   ├── 06_MLP.ipynb
│   └── 07_Model_Comparison.ip
├── results/
│   ├── Logistic_regression_metrics.csv
│   ├── Random_Forest_metrics.csv
│   ├── XGBoost_metrics.csv
│   ├── MLP_metrics.csv
│   └── Comparison_metrics.csv
├── figures/
│
├── requirements.txt
│
└── README.md
```

---

# 📊 Jeu de données

Le projet utilise un jeu de données simulant des transactions bancaires.

Le jeu de données contient :

- des transactions légitimes ;
- des transactions frauduleuses ;
- plusieurs variables décrivant les clients, les comptes et les transactions.

---

# ⚙️ Prétraitement des données

Le pipeline de préparation comprend :

- Nettoyage des données
- Gestion des valeurs manquantes
- Encodage des variables catégorielles
- Encodage cyclique des variables temporelles
- Standardisation avec StandardScaler
- Séparation Train / Validation / Test
- Création des DataLoader PyTorch

---

# 🤖 Modèles développés

## Machine Learning

- Régression Logistique
- Random Forest
- XGBoost

## Deep Learning

### Multi-Layer Perceptron (MLP)

Architecture finale :

```text
Entrée (45 variables)
        │
Couche cachée (64 neurones)
        │
ReLU
        │
Dropout (0.5)
        │
Couche de sortie (Sigmoid)
```

### Hyperparamètres retenus

| Paramètre | Valeur |
|-----------|--------|
| Architecture | [64] |
| Learning Rate | 0.0001 |
| Dropout | 0.5 |
| Weight Decay | 0.001 |
| Optimiseur | Adam |
| Fonction de perte | BCEWithLogitsLoss |
| Scheduler | ReduceLROnPlateau |
| Early Stopping | Oui |

---

# 📈 Métriques d'évaluation

Les modèles sont évalués à l'aide des métriques suivantes :

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Matrice de confusion
- Courbe ROC
- Courbe Precision-Recall

---

# 🚀 Installation

## Cloner le dépôt

```bash
git clone https://github.com/votre-utilisateur/Fraud-Detection-Project.git
```

## Se déplacer dans le projet

```bash
cd Fraud-Detection-Project
```

## Créer un environnement virtuel

```bash
python -m venv .venv
```

## Activer l'environnement

### Windows

```bash
.venv\Scripts\activate
```

### Linux / macOS

```bash
source .venv/bin/activate
```

## Installer les dépendances

```bash
pip install -r requirements.txt
```

---

# ▶️ Exécution

Les notebooks doivent être exécutés dans l'ordre suivant :

1. Exploration des données
2. Prétraitement des données
3. Régression Logistique
4. Random Forest
5. XGBoost
6. Optimisation du MLP
7. Entraînement du MLP final
8. Comparaison des modèles

---

# 📊 Résultats

Chaque modèle est évalué selon les mêmes métriques afin de garantir une comparaison équitable.

Le modèle final est sélectionné principalement selon :

- le ROC-AUC ;
- le Recall ;
- le F1-score ;
- la Precision.

Les résultats finaux sont regroupés dans le notebook **08_Model_Comparison.ipynb**.

---

# 🛠️ Technologies utilisées

- Python
- Pandas
- NumPy
- Scikit-learn
- PyTorch
- XGBoost
- Matplotlib
- tqdm
- Jupyter Notebook
- Git & GitHub

---

# 🔄 Pipeline du projet

```text
Jeu de données
       │
       ▼
Exploration des données
       │
       ▼
Prétraitement
       │
       ▼
Feature Engineering
       │
       ▼
Machine Learning
       │
       ├── Régression Logistique
       ├── Random Forest
       ├── XGBoost
       │
       ▼
Deep Learning (MLP)
       │
       ▼
Comparaison des modèles
       │
       ▼
Sélection du meilleur modèle
```

---

# 👨‍💻 Auteur

**Carlos Gael Taponjou Kenfack**


# 📄 Licence

Ce projet a été réalisé dans un contexte académique dans le cadre d'un projet du Certificat en DataScience. Il est destiné à des fins éducatives et de démonstration.

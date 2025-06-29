# 🏦 Bank Clients Churn

## 🎯 Objectif du projet

Ce projet a pour but de **prédire si un client d'une banque va clôturer son compte (churn)** ou rester fidèle.  
L'enjeu est d’anticiper ces départs afin de permettre à la banque de mettre en place des **stratégies de rétention ciblées**.

Nous utilisons un ensemble de données client comprenant des **caractéristiques démographiques, financières et comportementales** pour entraîner un modèle de machine learning capable de détecter les signaux de churn.

---

## 📊 Description des données

Le jeu de données contient les informations suivantes pour chaque client :

| Variable         | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| `CustomerId`     | Identifiant unique du client                                                |
| `Surname`        | Nom de famille du client                                                    |
| `CreditScore`    | Score de crédit                                                             |
| `Geography`      | Pays de résidence (France, Spain, Germany)                                 |
| `Gender`         | Genre (Male, Female)                                                        |
| `Age`            | Âge du client                                                               |
| `Tenure`         | Ancienneté dans la banque (en années)                                       |
| `Balance`        | Solde du compte                                                             |
| `NumOfProducts`  | Nombre de produits bancaires utilisés                                       |
| `HasCrCard`      | Possession d'une carte de crédit (1 = Oui, 0 = Non)                         |
| `IsActiveMember` | Membre actif ou non (1 = Oui, 0 = Non)                                      |
| `EstimatedSalary`| Salaire estimé                                                              |
| `Exited`         | **Cible** : le client a-t-il quitté la banque ? (1 = Oui, 0 = Non)          |



## 🧠 Approche

### 1. Exploration des données (EDA)
- Analyse des corrélations et de la distribution des variables  
- Visualisation des taux de churn selon les caractéristiques

### 2. Prétraitement
- Encodage des variables catégorielles  
- Normalisation des données numériques  

### 3. Modélisation
- Entraînement de plusieurs modèles :
  - Régression Logistique
  - Random Forest
  - XGBoost  
- Sélection du modèle le plus performant via validation croisée

### 4. Évaluation
- Utilisation de métriques adaptées :

## 📌 Résultats attendus

Un modèle capable de **prédire avec une bonne précision** si un client va quitter la banque ou non, tout en mettant en lumière les **facteurs influents**.  
Cela permettra aux décideurs de **prioriser certaines catégories de clients** pour les actions de fidélisation.

---

## 🛠️ Technologies utilisées

- **Python** : Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **Jupyter Notebook**  
- **Machine Learning** : classification supervisé

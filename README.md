
# 🧠 Data Mining Project – Analyse de Produits, Segmentation Clients & Analyse Temporelle

Ce projet explore les données d’un site e-commerce afin d’**analyser les produits**, **segmenter les clients**, et **étudier l’évolution temporelle des ventes**.  
Il se compose de **trois volets complémentaires** :

1. **Analyse de Produits** – identification des profils et anomalies produits  
2. **Segmentation des Clients & Détection d’Anomalies** – classification comportementale des clients  
3. **Analyse Temporelle des Produits & Embeddings** – exploration des tendances, saisonnalités et représentations vectorielles

---

## 🛍️ Partie 1 : Analyse de Produits

### 🎯 Objectif
Analyser le **comportement des produits** pour identifier les **anomalies**, regrouper les **profils similaires** et proposer des **recommandations commerciales**.

### 🧩 Données
Jeu **Online Retail II** (2009–2011) – plus d’un million de transactions e-commerce britanniques.  
Variables principales :  
`StockCode`, `Description`, `Quantity`, `UnitPrice`, `InvoiceDate`, `CustomerID`, `Country`.

### ⚙️ Méthodologie
1. **Prétraitement** : nettoyage et agrégation par produit (prix moyen, quantité, chiffre d’affaires, taux de retour).  
2. **Détection d’anomalies** :  
   - *Isolation Forest* → anomalies modérées  
   - *DBSCAN* → cas extrêmes (~2 % de produits exclus)  
3. **Segmentation (K-Means, GMM)** : identification de **4 profils produits** :  
   - **Dormants** : faible activité  
   - **Stars** : forte demande et ventes élevées  
   - **Premium** : prix élevés, faible rotation  
   - **Rotation moyenne** : ventes équilibrées

### 🧠 Outils
**Python** (pandas, scikit-learn, matplotlib), **Jupyter Notebook**, **Git/GitHub**.

---

## 👥 Partie 2 : Segmentation des Clients & Détection d’Anomalies

### 🎯 Objectif
Segmenter les **clients** selon leurs **comportements d’achat** et détecter les **transactions atypiques** afin d’améliorer la **compréhension** et la **fidélisation** client.

### ⚙️ Étapes principales
1. **Analyse RFM** : calcul de la **Récence**, **Fréquence** et **Montant** pour chaque client.  
2. **Clustering** : comparaison de **K-Means**, **DBSCAN** et **GMM** pour regrouper les clients en profils homogènes.  
3. **Détection d’anomalies** : utilisation d’**Isolation Forest** et **DBSCAN** pour repérer les comportements rares ou suspects.

### 📊 Résultats
- **K-Means** : segmentation claire et équilibrée.  
- **DBSCAN** : détection efficace des clients marginaux.  
- **GMM** : capture des comportements intermédiaires.  
- Les **anomalies détectées** concernent des montants, retours ou commandes inhabituels.

### 🧠 Outils
**Python**, **Pandas**, **Scikit-learn**, **Matplotlib**, **Seaborn**, **Jupyter Notebook**.

---



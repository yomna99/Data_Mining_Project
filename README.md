# 🛍️ Partie1: Analyse de Produits 

## 🎯 Objectif
Analyser le **comportement des produits** d’un site e-commerce afin d’identifier les **anomalies**, regrouper les **profils similaires** et formuler des **recommandations commerciales**.

---

## 🧩 Données
Jeu **Online Retail II** (2009–2011) – plus d’un million de transactions e-commerce britanniques.  
Variables : `StockCode`, `Description`, `Quantity`, `UnitPrice`, `InvoiceDate`, `CustomerID`, `Country`.

---

## ⚙️ Méthodologie
1. **Prétraitement** : nettoyage et agrégation par produit (prix moyen, quantité, chiffre d’affaires, taux de retour).  
2. **Détection d’anomalies** :  
   - *Isolation Forest* (anomalies modérées)  
   - *DBSCAN* (cas extrêmes) → ~2 % de produits exclus.  
3. **Segmentation (K-Means, GMM)** : 4 profils produits :  
   - **Dormants** : faible activité  
   - **Stars** : forte demande  
   - **Premium** : prix élevés, rotation faible  
   - **Rotation moyenne** : ventes équilibrées  

---

## 🧠 Outils
Python (pandas, scikit-learn, matplotlib), Jupyter Notebook, Git/GitHub.

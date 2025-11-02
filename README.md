# 🛍️ Partie1: Analyse de Produits – Data Mining Project

## 🎯 Objectif
Analyser le **comportement des produits d’un site e-commerce** afin d’identifier les **anomalies**, regrouper les **profils similaires** et fournir des **recommandations commerciales** basées sur les données.

---

## 🧩 Jeu de données
Données issues du **jeu Online Retail II** (2009–2011) : plus d’un million de transactions e-commerce britanniques.  
Variables clés : `StockCode`, `Description`, `Quantity`, `UnitPrice`, `InvoiceDate`, `CustomerID`, `Country`.

---

## ⚙️ Méthodologie
1. **Prétraitement** : nettoyage, uniformisation et agrégation au niveau produit  
   → indicateurs : prix moyen, quantité vendue, chiffre d’affaires, taux de retour.  
2. **Détection d’anomalies** :  
   - *Isolation Forest* → anomalies modérées  
   - *DBSCAN* → cas extrêmes  
   → environ **2 %** de produits suspects exclus.  
3. **Segmentation (K-Means, GMM)** : identification de **4 profils produits** :  
   - **Dormants** : faible activité  
   - **Stars** : forte demande et chiffre d’affaires élevé  
   - **Premium** : prix élevés, faible rotation  
   - **Rotation moyenne** : ventes équilibrées

---

## 🧠 Outils
- **Python** : pandas, scikit-learn, matplotlib  
- **Jupyter Notebook**  
- **Git & GitHub** pour la gestion de version  

---

## 📈 Résultats clés
- 1 067 371 transactions analysées  
- 5 616 produits agrégés  
- 113 produits anormaux détectés (~2 %)  
- 4 segments produits distincts et interprétables  

# Prédiction des Prix et Actifs du S&P 500 avec Machine Learning

Ce projet explore l'utilisation de diverses techniques de Machine Learning pour prédire les prix de clôture logarithmiques (`Log_Close`) de l'indice **S&P 500**. L'objectif est de fournir des outils permettant d’orienter des stratégies d’investissement sur cet indice de référence, en s’appuyant sur des données financières et économiques enrichies.

---

## 🔍 Contexte

Le **S&P 500** est un indice regroupant les 500 plus grandes entreprises cotées aux États-Unis, servant de baromètre clé pour mesurer la santé économique et les performances globales du marché. Ce projet combine des données historiques du S&P 500 avec des indicateurs macroéconomiques et techniques pour construire des modèles prédictifs robustes.

---

## 🎯 Objectifs

1. Analyser les tendances historiques des prix et des indicateurs économiques.
2. Développer plusieurs modèles de prédiction, incluant des modèles linéaires, des algorithmes basés sur les arbres de décision et des réseaux neuronaux récurrents.
3. Évaluer les performances des modèles en termes de précision et de robustesse.
4. Aider sur des stratégies d’investissement en S&P500.

---

## 🛠️ Méthodologie

1. **Collecte des données** :
   - Utilisation d'APIs comme **Yahoo Finance**, **FRED**, et **Alpha Vantage** pour récupérer les données financières et macroéconomiques.
2. **Transformation des données** :
   - Application de transformations logarithmiques pour stabiliser les variations des prix.
   - Création d'indicateurs techniques tels que le RSI et le MACD.
3. **Modélisation** :
   - Entraînement et évaluation des modèles suivants :
     - Régression linéaire
     - ARIMA
     - Random Forest
     - Gradient Boosting
     - Réseaux neuronaux LSTM
4. **Évaluation** :
   - Utilisation de métriques comme le **R²** et le **MSE** pour comparer les performances.

---

## 📊 Résultats

- **Régression linéaire** : Une capacité explicative limitée (R² = 0.177) mais des relations significatives identifiées, notamment avec `VIX` et `Log_RealGDP`.
- **ARIMA** : Le modèle ARIMA(2, 0, 0) capture efficacement les dépendances temporelles à court terme.
- **Random Forest** : Faible capacité explicative (R² = 0.136), nécessitant des variables plus pertinentes.
- **Gradient Boosting** : Performances négatives sur le jeu de test (R² < 0).
- **LSTM** : Performances prometteuses pour capturer les tendances principales, bien qu'améliorables avec des ajustements d’hyperparamètres.

---

## 📈 Stratégies d'investissement

1. **Indicateur VIX** : Identifier des périodes de forte volatilité pour anticiper des opportunités ou des risques.
2. **Modèles LSTM et ARIMA** : Exploiter les tendances prédites à long terme pour optimiser les décisions d'achat/vente.

---


## 📁 Structure du projet

- **notebook/** : Scripts et notebooks pour les analyses.
- **Rapport/** : explications détaillés et discussions des résultats.

---



## 📝 Auteurs

Développé par AKDI Oussama, étudiant en Data Science et Machine Learning.

---

### **Remarque :**
Pour ajouter ce fichier comme README dans votre dépôt GitHub, nommez-le `README.md`. Il sera automatiquement affiché sur la page principale de votre dépôt.

Si vous avez besoin de modifications ou d’ajouts, faites-le-moi savoir ! 😊

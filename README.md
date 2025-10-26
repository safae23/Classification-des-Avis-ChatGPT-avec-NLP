# Classification des Avis ChatGPT avec NLP

## Description du projet
Ce projet a pour objectif de **classifier automatiquement les avis laissés sur ChatGPT** (positifs, négatifs, neutres) en utilisant des **techniques avancées de traitement du langage naturel (NLP)** et des **réseaux de neurones profonds (RNN, LSTM, GRU)**.

Le notebook montre l’ensemble du pipeline : de la préparation des données jusqu’à l’évaluation des modèles.

---

## Technologies et bibliothèques utilisées
- 🐍 **Python 3.x**
- 🧩 **TensorFlow / Keras**
- 🧠 **Scikit-learn**
- 📊 **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**
- 🔤 **NLTK** (tokenisation, stopwords, lemmatisation)
- ☁️ **WordCloud** pour la visualisation des mots

---

## Structure du projet

---

## 🧪 Étapes du projet

### 1️⃣ Préparation et nettoyage des données
- Chargement du dataset `ChatGPT_Reviews.csv`
- Suppression des doublons et des valeurs manquantes
- Tokenisation, suppression des stopwords et lemmatisation

### 2️⃣ Analyse exploratoire (EDA)
- Distribution de la longueur des reviews  
- Visualisation des mots les plus fréquents à l’aide de **WordCloud**
- Répartition des classes (avis positifs/négatifs)

### 3️⃣ Modélisation
Plusieurs architectures de réseaux de neurones ont été testées :
- **SimpleRNN**
- **LSTM**
- **GRU**
- **Attention Layer** (pour améliorer la contextualisation des séquences)

Chaque modèle utilise :
- **Embedding Layer**
- **Dropout**
- **Dense Layers** pour la classification finale

### 4️⃣ Évaluation
- Matrice de confusion
- Rapport de classification (précision, rappel, F1-score)
- Courbes ROC et AUC pour la comparaison des modèles

---

## Résultats attendus
Les modèles LSTM et GRU montrent généralement les meilleures performances sur les données textuelles, avec une bonne capacité à capter le contexte des phrases.

Les métriques clés présentées :
- **Accuracy**
- **Recall**
- **F1-score**

---

## Visualisations
Quelques graphiques générés :
- Distribution de la longueur des reviews
- WordCloud des mots fréquents
- Matrice de confusion
- Courbe ROC

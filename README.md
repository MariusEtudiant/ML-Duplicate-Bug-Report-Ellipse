# ML-Duplicate-Ellipse

## Duplicate Bug Report Detection

**TP initialement créé par Irving Muller Rodrigues pour le cours de fouilles de données de Montréal.**

- **Date de remise** : 08/11/2024

---

## 📖 Présentation

Les bugs logiciels sont fréquents en raison de la complexité des systèmes. Pour gérer ces problèmes, les entreprises utilisent des systèmes de suivi des bugs (**BTS**), permettant aux développeurs, testeurs, et même utilisateurs de signaler de nouveaux bugs en remplissant un formulaire.

### 🐞 Les champs principaux d'un rapport de bug :
- **Données catégorielles** :
  - Exemples : composant, version, produit.
  - Ces champs acceptent des valeurs fixes provenant d'une liste d'options prédéfinies.
- **Résumé** et **description** :
  - Champ texte où les utilisateurs décrivent librement le bug.
  - Contraintes : le résumé a une limite maximale de caractères.

### ⚠️ Problème : Les rapports de bugs en double
Le manque de communication et de synchronisation entre utilisateurs peut entraîner la soumission répétée d’un même bug. Cela complique la gestion des bugs et alourdit les processus de suivi.

### 🎯 Objectif du TP
Développer un système capable de prédire si une **paire de rapports de bug soumis** sont **dupliqués** ou non. Ce système pourra être intégré dans un BTS pour identifier automatiquement les rapports dupliqués et améliorer la gestion des bugs.

---

## 💾 Fichier de données
- Les données nécessaires sont disponibles sous forme d'un fichier JSON (disponible sur demande).

---

## 🔧 Technologies et outils suggérés
- **Python** : pour le traitement des données et le développement du modèle.
- **Bibliothèques suggérées** :
  - `scikit-learn` pour les modèles de machine learning.
  - `pandas` et `numpy` pour le traitement des données.
  - `matplotlib` et `seaborn` pour la visualisation.
  - `beautifulsoup` pour le scrapping des données.

---

## ✍️ Auteur original
**Irving Muller Rodrigues**

---

Si vous avez des questions ou besoin d'assistance, n'hésitez pas à demander ! 😊

# 📝 Compte rendu d’analyse — Dataset Amazon

## 1. 📥 Importation des données

Les données ont été importées depuis un fichier CSV (`amazon.csv`).  
Premières vérifications effectuées :

- Aperçu des 5 premières lignes  
- Informations sur les types de colonnes  
- Dimensions du dataset  
- Détection des doublons  
- Recherche de valeurs manquantes  

---

## 2. 🧹 Nettoyage des données

### 2.1. Suppression des doublons
Les doublons détectés ont été supprimés.

### 2.2. Conversion des types

- `discounted_price` : suppression du symbole ₹ et des virgules, conversion en float  
- `actual_price` : idem  
- `discount_percentage` : suppression du `%`, conversion en float  
- `rating` : conversion en numérique avec gestion d’erreurs  
- `rating_count` : suppression des séparateurs de milliers, conversion en int  

### 2.3. Gestion des valeurs manquantes  
- Colonnes numériques → imputation par la **moyenne**  
- Colonnes catégorielles → imputation par le **mode**  

---

## 3. 📊 Vérification post-nettoyage

- Absence de doublons  
- Plus de valeurs manquantes  
- Types de colonnes convertis correctement  
- Dimensions du dataset mises à jour  
- Aperçu visuel des premières lignes du dataset nettoyé  

---

## 4. 🔍 Analyse exploratoire

### 4.1. Matrice de corrélation
Une matrice de corrélation a été générée pour étudier les liens entre les variables numériques.

### 4.2. Régression linéaire
Une régression linéaire simple a été effectuée avec :

- Variable explicative : première colonne numérique  
- Variable cible : seconde colonne numérique  

Résultats :

- Coefficient (pente)  
- Ordonnée à l’origine  
- Score R²  

Un graphique incluant la droite de régression a été généré.

---

## 5. 🤖 Régression logistique

Un dataset de classification synthétique a été généré pour entraîner un modèle de régression logistique.

### 5.1. Coefficients calculés

- `w0` : coefficient lié à Feature_X  
- `w1` : coefficient lié à Feature_Y  
- `b` : intercept  

### 5.2. Visualisation

La figure comprend :

- Les points des classes 0 et 1  
- Les zones de décision  
- La droite de séparation  
- L’équation affichée sur le graphique  

### 5.3. Performance

- Accuracy du modèle affichée après entraînement  

---

## 6. ✅ Conclusion

Le script a permis :

- D’importer et nettoyer correctement les données  
- De réaliser une analyse exploratoire complète  
- De tester deux modèles : régression linéaire et logistique  
- De produire des visualisations exploitables  

Le dataset est désormais totalement prêt pour une modélisation plus avancée.



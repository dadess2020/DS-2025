<img src="WhatsApp Image 2025-12-03 at 14.25.26.jpeg" style="height:464px;margin-right:432px"/>
DADESS ANASS cac 1

# Analyse Fictive du Dataset

## 1. Introduction
Cette analyse fictive présente un aperçu rapide du dataset utilisé, ainsi que deux modèles :  
- une régression linéaire  
- une régression logistique  

Les résultats sont illustrés par les graphiques correspondants.

---

## 2. Statistiques Générales
Le dataset contient **n observations** décrivant plusieurs caractéristiques musicales.  
Les variables principales montrent une dispersion modérée, cohérente avec des données audio.

---

## 3. Corrélation
La matrice de corrélation révèle quelques relations notables :  
- une corrélation positive entre `energy` et `loudness`  
- une corrélation négative entre `acousticness` et `energy`  
- une faible corrélation entre `tempo` et les autres variables  

Ces relations guident le choix des variables pour les modèles prédictifs.

---

## 4. Régression Linéaire
La régression linéaire a été appliquée entre :  
- **X : `energy`**  
- **Y : `loudness`**

### 🟦 Interprétation  
La droite ajustée montre une **tendance croissante** :  
plus une piste est énergique, plus son niveau sonore est élevé.

### 📈 Droite estimée  
\[
\hat{y} = a \cdot x + b
\]

### 📊 Illustration  
*(Graphique fictif — régression linéaire)*  
<img src="Capture d'écran 2025-12-03 141844.png" style="height:464px;margin-right:432px"/>

---

## 5. Régression Logistique
La régression logistique a été utilisée pour prédire :  
- **Variable cible binaire : `hit` (0 = non, 1 = oui)**  
- **Variable explicative : `popularity`**

### 🟩 Interprétation  
La probabilité qu'une musique soit un “hit” **augmente fortement** avec la popularité.  
La courbe logistique montre une transition nette autour d’un seuil critique.

### 📈 Fonction logistique  
\[
P(hit=1) = \frac{1}{1 + e^{-(\beta_0 + \beta_1 x)}}
\]

### 📊 Illustration  
*(Graphique fictif — régression logistique)*  
<img src="Capture d'écran 2025-12-03 141836.png" style="height:464px;margin-right:432px"/>

---

## 6. Conclusion
- La relation `energy → loudness` est clairement linéaire.  
- La variable `popularity` est un bon indicateur logistique pour prédire les “hits”.  
- L’analyse fictive confirme la cohérence des données et illustre les deux modèles couramment utilisés en data science.


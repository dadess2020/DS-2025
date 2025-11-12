## Contexte et Objectifs

L’étude porte sur l’analyse des [paiements par défaut des clients de cartes de crédit à Taïwan], avec un jeu de données comprenant 30 000 clients et 23 variables numériques. L’objectif est d’évaluer la capacité de six méthodes d’exploration de données à estimer précisément la probabilité de défaut, critère essentiel en gestion du risque de crédit.

## Méthodologie

- Utilisation du [Sorting Smoothing Method] pour estimer la probabilité réelle de défaut.
- Prédiction de la probabilité de défaut par six approches de data mining, dont le réseau de neurones artificiels, l’arbre de décision, l’analyse discriminante, la régression logistique et le KNN.
- Régression linéaire simple (\(Y = A + BX\)) entre la probabilité réelle estimée (\(Y\)) et la probabilité prédite (\(X\)), afin d’évaluer la qualité des prédictions.

## Caractéristiques du Jeu de Données

| Caractéristiques         | Description                      |
|-------------------------|----------------------------------|
| Nombre d’instances      | 30 000 clients                   |
| Nombre de variables     | 23 (entière, réelle)             |
| Domaine d’application   | Business (gestion du risque)     |
| Tâche associée          | Classification                   |

## Résultats des Méthodes Comparées

| Méthode                    | Coefficient de détermination (\(R^2\)) | Intercept (A) | Slope (B) | Remarque principale                                   |
|---------------------------|-------------------|-------------|----------|------------------------------------------------------|
| Réseau de neurones        | **Plus élevé**    | ≈ 0         | ≈ 1      | Meilleure adéquation, estimation fidèle et non biaisée|
| Arbre de décision         | Élevé             | Variable    | Variable | Précision notable, sensible au bruit                 |
| Analyse discriminante     | Modéré            | Variable    | Variable | Méthode classique, moins performante que l’ANN       |
| Régression logistique     | Modéré            | Variable    | Variable | Robuste, mais moins précis que ANN ou arbres         |
| K-plus proche voisin (KNN)| Modéré            | Variable    | Variable | Précision variable selon paramétrage                 |
| Méthodes d’ensemble       | Élevé             | Variable    | Variable | Souvent plus précises, complexité accrue             |

*ANN : réseau de neurones artificiels.

## Importance et Perspectives

- Les réseaux de neurones surpassent généralement les approches classiques (régression logistique, analyse discriminante) pour la prédiction du risque de crédit grâce à leur capacité d’apprentissage adaptative et leur précision supérieure.
- La modélisation précise de la probabilité de défaut favorise une meilleure gestion des risques et prise de décision pour les institutions financières.
- L’intégration de méthodologies avancées via le data mining ouvre des perspectives innovantes pour le scoring et la personnalisation des offres de crédit.


# Mini projet : Prédiction des feux de forêt (Forest Fires) 
# Contexte Scientifique 
Les feux de forêt sont influencés par des indices météorologiques (FWI - Fire Weather 
Index) qui combinent humidité, vent et température. Prédire la surface brûlée est un 
défi majeur pour la gestion des secours. 
# Objectif 
Prédire la surface brûlée (variable 'area') à partir des indices météo (FFMC, DMC, DC, 
ISI) et des conditions instantanées. 
Tâches à réaliser 
1. Contexte : Indices de danger incendie et météorologie. 
2. Données : Comprendre les indices FWI et la distribution très asymétrique de la 
variable 'area'. 
3. Transformation : Appliquer une transformation Log(x+1) à la variable cible 'area'. 
4. Corrélations : Corrélation entre Température/Vent et Surface brûlée. 
5. Régression (Base) : Linear Regression sur données transformées. 
6. Régression (Non-linéaire) : SVM Regression (SVR) et KNN Regression. 
7. Classification (Variante) : Transformer le problème en binaire : "Feu majeur" (> 
0 ha) vs "Petit feu". 
8. Évaluation : Comparer RMSE sur la régression et Accuracy sur la classification. 
9. Interprétation : Difficulté de prédiction des événements extrêmes. 
# Exercices bonus
Ne garder que les 4 variables les plus pertinentes. 
Comparer les résultats avec et sans transformation logarithmique.
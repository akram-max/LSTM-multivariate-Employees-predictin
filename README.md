# LSTM-multivariate-Employees-predictin
Employees minotoring

L’entreprise souhaite disposer d’un outil d’aide à la décision permettant de qualifier le rendement de chaque collaborateur et de prédire son taux atteint pour le mois prochain. Il s’agit de choisir le meilleur modèle permettant de réaliser ce besoin.
Pour être entrainer, le modèle LSTM demande au moins 10 employés avec leurs performances étalée sur 6 mois (5 mois successifs et le dernier mois le plus récent comme cible ).

Pour faire la prédiction, les modèle LSTM ont besoin que les données soit complètes sur un ensemble des 5 mois les plus récents pour un employé donné : puisque c’est difficile, on a recours à l'interpolation et la moyenne pour combler les vides. 

Aussi, on a une exigence lors de l'apprentissage avec le mois du test qui doit exister et ne peut être interpolé.

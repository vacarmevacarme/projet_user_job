# Objectif

L'objectif est d’entraîner un modèle capable de prédire un taux de compatibilité entre un utilisateur et une offre d'emploi, en fonction de son parcours et des caractéristiques de l'offre (features).

Pour cela, la data set feedbacks est fondamental. On y trouve des **couples users/jobs** (features X) qui nous donnent un **résultat** *"viewed, applied, hired"* (y) que l'on cherchera à reproduire. On pourra donc entraîner notre modèle sur ces couples.

En phase de prédiction, nous fournirons au modèle une table de tous les couples possibles **test_users/jobs** pour obtenir un score et sélectionner les offres d'emploi qui obtiendront les meilleurs scores pour chaque user, ou aucun si le score passe en dessous d'un certain seuil. 

Nous évaluerons d'abord la qualité et les caractéristiques des données pour identifier un modèle qui est compatible avec nos objectifs. Nous identifierons ensuite les données utiles à notre modèle, ce qui guidera également notre nettoyage et transformation des données. Enfin, nous évoquerons les stratégies d'entrainement, d'évaluation et les risques éventuels. Cet exercie a pour but d'imaginer un modèle fonctionnel en peu de temps. Nous utiliserons donc un minimum de données pour cela pour n'avoir que peu de preprocessing.
# Project7

 Implémentez un modèle de scoring

Ce projet a pour objectif de créer une API afin de prédire l’attribution d’un prêt ou non à un client, tout en visualisant les données dans un dashboard interactif destiné au banquier et/ou client. 

Pour cela, le notebook dans le répertoire principal montre le développement du modèle utilisé dans l'API de prédiction, à l'aide des données disponibles à ce lien : https://www.kaggle.com/c/home-credit-default-risk/data. Les modèles ont été trackés et enregistrés via MLflow. Une analyse du datadrift a été effectuée à l'aide de la librairie Evidently. Le fichier .html est joint dans le répertoire principal.

L'API, développée à l'aide de Flask, est stockée dans le sous-repertoire "Flask". Ce répertoire contient les données utilisées pour la modèlisation, le modèle lui-même, l'application app.py, le Procfile et également un repertoire "tests" pour l'exécution des tests à l'aide de Pytest. 

Le dashboard, développé à l'aide de la libraire Streamlit, est stocké dans le répertoire "Dashboard".

Chacun de ces dossiers possède un fichier requirements.txt permettant d'installer les librairies nécéssaires à l'exécution du dashboard et de l'API.

Enfin, les deux applications (dashboard et API) sont deployées sur le cloud (Heroku) à l'aide d'un workflow de déploiement continu (Github Actions), intégrant les tests faits sur l'API.

Les url des deux applications sont :  
API :  https://frozen-cove-50105-311e5794eba1.herokuapp.com/
Dashboard : https://stark-bastion-85001-dd9a288dd2cb.herokuapp.com/

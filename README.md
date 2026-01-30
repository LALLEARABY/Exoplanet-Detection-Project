Détection d'Exoplanètes à partir des données du Télescope Spatial Kepler

1. Aperçu du Projet

Ce projet vise à identifier des exoplanètes en utilisant la Méthode du Transit. Lorsqu'une planète passe devant son étoile hôte, elle provoque une baisse infime et périodique de la luminosité de l'étoile.

Le défi principal de ce jeu de données est le déséquilibre extrême des classes : sur des milliers d'étoiles, seule une poignée possède des exoplanètes confirmées. Notre solution se concentre sur la maximisation du Rappel (Recall), garantissant qu'aucune découverte potentielle n'est ignorée par le système automatisé.

2. Caractéristiques Clés

Ingénierie des Caractéristiques (Feature Engineering) : Utilisation de la Transformée de Fourier Rapide (FFT) pour convertir l'intensité lumineuse du domaine temporel vers le domaine fréquentiel, révélant les rythmes orbitaux cachés.

Extracteurs Statistiques Avancés : Calcul de l'asymétrie (skewness), de l'aplatissement (kurtosis) et du rapport signal/bruit pour distinguer le bruit cosmique des véritables transits.

Modélisation d'Ensemble : Combinaison de modèles Random Forest et XGBoost (avec pondération des coûts) pour gérer le déséquilibre des classes de 1:100.

Impact Astronomique : Atteinte d'un Rappel de 100% sur l'ensemble de test, réduisant la charge de travail de vérification manuelle pour les astronomes de plus de 90%.

3. Structure du Répertoire

EXOPLANET_DETECTION.ipynb : Le notebook complet du projet incluant le nettoyage des données, l'EDA, la modélisation et l'interprétation des résultats.

requirements.txt : Liste des bibliothèques Python nécessaires pour reproduire les résultats.

4. Comment l'utiliser

Cloner le répertoire :

git clone [https://github.com/LALLEARABY/Exoplanet-Detection-Project.git](https://github.com/LALLEARABY/Exoplanet-Detection-Project.git)


Installer les dépendances :

pip install -r requirements.txt


Exécuter le Notebook : Ouvrez le fichier .ipynb dans Google Colab ou Jupyter Lab. Assurez-vous d'avoir les fichiers exoTrain.csv et exoTest.csv dans votre répertoire de travail.

5. Jeu de Données

Les données utilisées dans ce projet proviennent de la mission Kepler de la NASA.
Elles sont disponibles sur
[[kepler-labelled-time-series-data](https://www.kaggle.com/datasets/keplersmachines/kepler-labelled-time-series-data)]

Auteur: LALLE BABA ARABIE
Date: January 2026

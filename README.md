Projet MLP - INF3721

Ce projet, intitulé "Perceptron Multi-Couche (MLP)", est réalisé dans le cadre du cours "Apprentissage Supervisé et Non Supervisé I" (INF3721) à l'Université de Yaoundé 1, Département d'Informatique, Licence 3 en Data Science.
Équipe

    Lonsti Lambou Ronaldino (Matricule: 21T2271)
    Ndonkou Franck (Matricule: 21T2254)
    Tchiaze Fouosso Romero (Matricule: 21T2474)
    Djampa Njuitcha Anicet (Matricule: 21T2692)

Objectif

Ce projet vise à construire et entraîner un modèle de Perceptron Multi-Couche (MLP) pour la classification d'images à partir de l'ensemble de données CIFAR-10. L'objectif principal est de prédire la classe (parmi 10 classes) à laquelle chaque image appartient.
Contenu du Projet

    Script Python: Le script principal du projet est fourni dans le fichier MLP_CIFAR10.py. Ce script contient l'ensemble du code nécessaire pour charger les données, construire et entraîner le modèle MLP, évaluer les performances du modèle et effectuer des prédictions sur de nouvelles données.
    Modèle Enregistré: Le modèle entraîné est sauvegardé au format HDF5 dans le fichier modele_pml.h5.
    Makefile: Le fichier Makefile est fourni pour faciliter la compilation et l'exécution du script Python.
    Documentation: Ce fichier README sert de documentation pour le projet, fournissant des instructions sur la façon d'exécuter le code, des explications sur l'architecture du modèle, l'optimiseur utilisé, la fonction de perte, etc.

Instructions d'Exécution

Pour exécuter le script Python, assurez-vous d'avoir Python 3 installé sur votre système, ainsi que les bibliothèques requises (TensorFlow, NumPy, Matplotlib, etc.). Vous pouvez installer les dépendances en exécutant pip install -r requirements.txt.

Ensuite, exécutez le script principal à l'aide de la commande suivante :

bash

python MLP_CIFAR10.py

Architecture du Modèle

Le modèle MLP utilisé dans ce projet est composé de plusieurs couches cachées, avec différentes fonctions d'activation. Voici l'architecture du modèle :

    Couche Dense avec 200 neurones et activation tanh
    Couche Dense avec 200 neurones et activation tanh
    Couche Dense avec 300 neurones et activation sigmoid
    Couche Dense avec 300 neurones et activation relu
    Couche Dense avec 200 neurones et activation tanh
    Couche Dense avec 300 neurones et activation sigmoid
    Couche de sortie Dense avec 10 neurones (pour les 10 classes) et activation softmax

Évaluation du Modèle

Le modèle est entraîné sur 100 époques avec une taille de lot de 10000. Les performances du modèle sont évaluées à l'aide de la perte d'entropie croisée catégorielle et de la précision. La précision finale du modèle sur l'ensemble de test est affichée dans la sortie.
Fichiers Additionnels

    Répertoire src: Contient les fichiers source du projet, notamment MLP_CIFAR10.py.
    Répertoire obj: Contiendra les fichiers objets générés lors de la compilation.
    Répertoire bin: Contiendra les exécutables générés lors de la compilation.


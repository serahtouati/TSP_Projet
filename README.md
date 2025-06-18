# TSP_Projet – Problème du Voyageur de Commerce

Ce projet a été réalisé dans le cadre d’un travail universitaire en L3 Mathématiques-Informatique à l’Université d’Aix-Marseille. Il consiste à résoudre le problème du voyageur de commerce (Traveling Salesman Problem, TSP) sur un ensemble de villes françaises, à l’aide de plusieurs heuristiques.

## Objectifs

Trouver un chemin passant une seule fois par chaque ville d’un ensemble donné, et revenant au point de départ, tout en minimisant la distance totale parcourue. 

## Données utilisées

Les données proviennent d’un fichier CSV contenant une sélection de villes françaises avec leurs coordonnées géographiques :  
"data/fr.csv"(https://github.com/serahtouati/TSP_Projet/blob/main/data/fr.csv)

## Fonctionnalités du notebook

Le notebook "TSP_Projet.ipynb"(https://github.com/serahtouati/TSP_Projet/blob/main/TSP_Projet.ipynb) contient toutes les étapes suivantes :

1. Chargement des données et sélection des villes  
2. Calcul de la matrice des distances (Haversine)  
3. Implémentation de l’heuristique du plus proche voisin  
4. Amélioration du chemin via l’algorithme 2-opt  
5. Implémentation complète d’un algorithme génétique avec :
   - Génération de population  
   - Fonction de fitness  
   - Crossover (Order Crossover)  
   - Mutation  
   - Sélection par tournoi  
6. Visualisation des trajets calculés avec matplotlib

## Résultats

Les performances des différentes heuristiques ont été évaluées sur plusieurs échantillons de villes. Les résultats montrent que :

  L’algorithme du plus proche voisin fournit rapidement une solution initiale, mais souvent sous-optimale.

  L'algorithme 2-opt permet une nette amélioration de la solution de départ avec un faible coût computationnel.

  L'algorithme génétique fournit les meilleurs résultats en termes de longueur totale du trajet, mais au prix d’un temps de calcul plus important.


## Technologies utilisées

Python  
Google Colab  
Pandas / NumPy  
Matplotlib



Projet réalisé par Yael Israel , Myriam Germon , Eden Nahoum  et Serah Touati.

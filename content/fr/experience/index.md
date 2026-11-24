---
title: "Expériences"
description: "Description d'expériences recherches et professionnelle."
featured_image: '/images/mountain_style.jpg'
menu:
  main:
    weight: 3
---

Une description de mes expériences antérieure:

---

#### Avril 2022 - Novembre 2023: Chercheur post-doctoral en biologie computationnelle, Université de Montpellier, Montpellier, France
- Objectifs:
    + mieux comprendre comment une cellule isolée (cellule fécondée) peut se transformer en un organisme biologique complexe
    + modéliser la morphologie d’un embryon, principalement la forme, en utilisant la description historique du développement des cellules
- Résultats:
    + représentation de la forme des cellules embryonnaires comme des paramètres d’un diagramme de Voronoï pondéré sphérique
    + transfert de MATLAB à Python du logiciel d’optimisation qui extrait les paramètres de diagramme à partir d’images d’embryons, afin d'exécuter les calculs sans restriction sur le supercalculateur Jean Zay
    + ajout d’un traitement des cellules en forme de cacahuète et de l’initialisation améliorée des paramètres pour construire plus précisément le diagramme de Voronoï pondère sphérique
    + réalisation d'un système logiciel permettant de stocker dans une base de données Neo4j et de traiter les paramètres des diagrammes calculés et les marqueurs biologiques des cellules
    + description de l’évolution des paramètres du diagramme liés au processus de développement et pour différents embryons, comme trajectoires multidimensionnelles dans l’espace
    + création d’un réseau neuronal, en utilisant le logiciel Transtab, pour prédire la dynamique de la forme cellulaires et la probabilité de la division en l’étape suivante basée sur l’histoire récente du développement des cellules et les trajectoires construites, les résultats montrent qu’il est possible de prédire la probabilité de division cellulaire avec une précision de 82%
- compétences:
    + Biologie computationnelle, Morphologie, Diagrammes de Voronoı̈, Traitement d’images, Apprentissage automatique, Base de données orientée graphe
- logiciels:
    + Python, NumPy, SciPy, Scikit-image, Matplotlib, Miniconda, Pandas, TensorFlow, Transtab, PyCharm, MATLAB, Neo4j, Cypher, Ubuntu Linux, Bash, Git

---

#### Mai 2017 - Septembre 2021: Doctorant, Ingénieur en recherche, INRIA, Université de Strasbourg, Strasbourg, France
- Objectifs:
    + estimer les conditions aux limites du foie pour améliorer la précision de la simulation en cas d’un système de réalité augmentée en chirurgie hépatique
    + simuler un comportement réaliste du foie, une influence d’organes et des tissus environnants en temps réel
- Résultats:
    + construction d’une méthode à éléments finis hyperélastiques pour les déformations du foie et le système ressort cubique pour les conditions aux limites
    + développement d’un composant logiciel qui décrit des ressorts avec la relation polynomiale entre la contrainte et la déformation et qui a été intégré dans le logiciel SOFA
    + participation à la création d’un module logiciel pour estimer des paramètres différents des modèles à l’aide des filtres de Kalman non linéaires
    + réalisation d’une approche basée sur un filtrage de Kalman dit "unscented" d’ordre réduit comme le meilleur choix pour le compromis performance/précision en temps réel
    + segmentation et extraction de marqueurs à partir d'une séquence d'images RGB-D afin d'obtenir des observations pour le processus d'estimation
    + construction d’une optimisation basée sur un préconditionneur afin d’améliorer l’efficacité du processus d’estimation (le temps de calcul est réduit de 26%)
    + création d’une approche basée sur l’enregistrement déformable des formes du foie (cartographie métrique difféomorphe à grande déformation) pour obtenir des statistiques sur les positions des ligaments
    + élaboration des expériences basées sur des données synthétiques (l'erreur est réduite de 66\%) et réelles (l'erreur est réduite de 23\%) pour montrer l'amélioration de la précision dans les simulations avec des conditions aux limites estimées
- compétences:
    + Réalité augmentée, Simulation numérique, Méthode des éléments finis, Système masse-ressort, Filtrage Kalman, Cartographie métrique difféomorphe
- logiciels:
    + C++, STL, Eigen, OpenCV, PCL, SOFA, FEBio, Qt, CMake, QtCreator, Python, NumPy, Matplotlib, Deformetrica, Ubuntu Linux, Bash, Git

---

#### Mai 2014 - Novembre 2016: Ingénieur en développement logiciel et en recherche, Filière scientifique et production Energiya, Usine Energiya, Saint-Pétersbourg, Russie
- Objectifs:
    + développer des modules pour trouver des signaux divers dans le spectre des ondes radio, maintenir la base de données pour garder les éléments détectés dans les enregistrements, collecter des statistiques sur les caractéristiques des signaux à l’aide des outils d’analyse
- Résultats:
    + emploi d’un module logiciel qui analyse l’apparence du signal semblable au bruit et recueille l’information de base
    + transfert de MATLAB à C++ d’un module qui recherche des signaux à spectre étalé par saut de fréquence et extrait les paramètres de base
    + réalisation d'un composant qui enregistre les informations sur les signaux détectés et à leurs paramètres dans une base de données PostgreSQL
    + développement d’une interface graphique pour afficher la fréquence et le balayage spectral des données, ainsi que les positions des signaux détectés
- compétences:
    + Traitement numérique du signal, Analyse de Fourier, transformation de Fourier rapide
- logiciels:
    + C++, Intel IPP, STL, Boost, Qt, CMake, Visual Studio, SQL, PostgreSQL, MATLAB, MS Windows, Git

---

#### Août 2010 - Février 2014: Ingénieur en développement logiciel, Bodynova, Saint-Pétersbourg, Russie
- Objectifs:
    + développer un logiciel serveur et client pour modéliser la forme du corps d’un patient et les résultats des interventions en chirurgie d’implant et d’extenseur mammaires
    + modéliser de manière réaliste les propriétés biomécaniques de la peau, du tissu adipeux, des muscles, des os et des implants
- Résultats:
    + emploi du logiciel qui modélise le placement d’implant dans les tissus mous, estimation de la précision des résultats et du temps de calcul
    + élaboration d’une interface graphique pour le logiciel de modélisation permettant de choisir un implant du catalogue et spécifier les paramètres de la position
    + construction d'un système masse-ressort innovant multicouche, non linéaire et anisotrope, réalisé comme un module logiciel en C++, pour décrire la déformation des tissus mous
    + réalisation d'un composant de rendu basé sur OpenGL pour observer le comportement du système masse-ressort
    + développement de la modification d’un modèle de voxels pour accélérer le traitement des collisions entre les implants et les tissus mous
- compétences:
    + Réalité virtuelle, Simulation numérique, Système masse-ressort, Traitement d’images, Géométrie computationnelle, Graphisme 3D
- logiciels:
    + C++, STL, WildMagic, WxWidgets, OpenCV, Bullet physics engine, OpenGL, OGRE, Visual Studio, HTML/CSS, JavaScript, Wolfram Mathematica, MS Windows, SVN

---

#### Juillet 2008 - Juillet 2010: Stagiaire, Ingénieur en développement logiciel inférieur, Corporation EMC, Saint-Pétersbourg, Russie
- Objectifs:
    + participer au développement d’un nouveau système de stockage
- Résultats:
    + développement d'un composant de pilote de bas niveau pour le système de stockage de données, notamment un mécanisme d'accès direct au disque (Bypass I/O) et un module permettant de sauvegarder le cache de données en cas d'arrêt d'urgence
    + configuration du matériel de quatre nouveaux systèmes de stockage pour avoir la connexion d’accès à distance
- compétences:
    + Pilotes de périphériques de stockage, Développement sous Linux
- logiciels:
    + C, gdb, make, Valgrind, Linux utils, Vim, Perl, Linux, SVN

---


[Retour]({{< ref "experience/index.md" >}})

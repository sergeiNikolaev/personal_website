---
title: "Recherche"
description: "Description de mon travail des recherches."
featured_image: '/images/mars_style.jpg'
menu:
  main:
    weight: 4
---

## Enquête sur le développement de l’embryon

Comme un chercheur postdoctoral, j’ai participé à un projet lié à l’analyse du processus qui décrit le développement des embryons. L’idée principale du travail est d'essayer de mieux comprendre comment une cellule fécondée se transforme en un organisme biologique complexe. Pour la recherche, des embryons [acsidiens](https://fr.wikipedia.org/wiki/Ascidiacea) ont été utilisés parce que le processus de développement a une structure simple. La structure de l’embryon dans l’espace a été approximée avec [un diagramme de Voronoï](https://fr.wikipedia.org/wiki/Diagramme_de_Vorono%C3%AF) pondéré sphérique. Ce modèle décrit la forme de l'embryon avec une précision suffisante, mais il possède un peu de paramètres (cinq paramètres pour une cellule) pour la représenter. Par conséquent, la complexité du système est réduite. Pour illustrer le processus de développement, les paramètres de Voronoï ont été combinés dans des trajectoires multidimensionnelles. Les trajectoires ont ensuite été analysées et visualisées en utilisant les méthodes de réduction dimensionnelle. Un réseau neuronal a également été entraîné pour donner une prédiction de la trajectoire d’embryon. Toutefois, les résultats ont montré qu’il est nécessaire de poursuivre l'investigation et l'amélioration du système.

---

## Estimation des conditions aux limites pour améliorer la précision de la simulation

J’ai [écrit](https://theses.hal.science/tel-03416443) et [soutenu](https://www.youtube.com/watch?v=SYzDmdZIWF0) avec succès ma thèse de doctorat. La thèse était une partie de grand projet, l’idée de qui est créé un système de navigation pour la chirurgie du foie. L'objectif principal de mon travail est d'estimer des conditions aux limites du tissu hépatique pour améliorer la précision de la simulation. Les conditions aux limites prennent un rôle essentiel dans la capacité prédictive du modèle biomécanique. Cependant, en cas de foie, elles correspondent principalement aux ligaments, aux vaisseaux sanguins et aux organes environnants, dont les propriétés ont une description qui est spécifique au patient et ne peuvent être mesurées de manière fiable. On propose à modéliser les conditions aux limites comme [un système masse-ressort](https://fr.wikipedia.org/wiki/Syst%C3%A8me_masse-ressort) non linéaire et à estimer les paramètres.

Tout d'abord, on définit une approximation initiale généralisée. Les positions des ligaments ont récupéré d’un atlas statistique. Pour construire l’atlas, [une méthode de cartographie métrique difféomorphique à grande déformation](https://www.sciencedirect.com/science/article/abs/pii/S1053811914005205?via%3Dihub), qui est disponible dans [le logiciel Deformetrica](https://www.deformetrica.org), est appliquée à l’ensemble de modèles avec des ligaments segmentés. Les paramètres des ligaments sont calculés en utilisant la loi constitutive disponible dans la littérature et [le plugiciel d’optimisation](https://help.febio.org/docs/FEBioUser-4-1/UM41-Chapter-7.html) de [logiciel FEBio](https://febio.org).

La deuxième partie, c’est estimation de paramètres des ressorts basés sur résultats de la modélisation des ligaments. Et ensuite, on corrige l'approximation (le modèle du foie autant que des ligaments présentés comme des ressorts attachés) basée sur les données obtenues par une modalité pendant la chirurgie. L'estimation des paramètres et les corrections sont effectuées en utilisant [un filtre Kalman](https://fr.wikipedia.org/wiki/Filtre_de_Kalman) non linéaire, qui est disponible dans [le plugiciel Optimus](https://github.com/sofa-framework/Optimus), la partie de [logiciel SOFA](https://www.sofa-framework.org).

Pour évaluer l'approche proposée, on a réalisé quelques expériences sur des scénarios avec des données synthétiques et réelles. Les résultats montrent que, pour les scénarios avec des conditions aux limites estimées, il y a une certaine amélioration de la précision de la simulation.

#### Référence de la thèse

Nikolaev S. _Identification et caractérisation des conditions aux limites pour des simulations biomécaniques patient-spécifiques_, 2021 [Mémoire](https://theses.hal.science/tel-03416443) [Présentation de soutenance](https://www.youtube.com/watch?v=SYzDmdZIWF0)&ensp;&ensp;&ensp;&ensp;&ensp;[Plugiciel Optimus](https://github.com/sofa-framework/Optimus)

### Publications

1. Nikolaev S., Cotin S. _Estimation des conditions aux limites pour modélisation du foie patient spécifique pendant la chirurgie augmentée._ Journal international de radiologie et de chirurgie assistées par ordinateur, Vol. 15, №. 7, pp. 1107-1115, 2020 [Lien de journal](https://link.springer.com/article/10.1007/s11548-020-02188-x) [Lien d'archive](https://hal.archives-ouvertes.fr/hal-02634875/document) [Lien de présentation](https://www.youtube.com/watch?v=dztaapzOQqQ)

2. Mendizabal A., Tagliabue E., Hoellinger T., Brunet J.-N., Nikolaev S., Cotin S. _Simulation basée sur les données pour la chirurgie augmentée._ In: Développement et approches nouvelles en biomécanique et métamatériaux, Chap. 5, pp. 71-96, 2020 [Lien de journal](https://link.springer.com/chapter/10.1007/978-3-030-50464-9_5) [Lien d'archive](https://hal.inria.fr/hal-02538101/document)

3. Teaniti A., Brunet J.-N., Nikolaev S., Wang C., Edwin B., Cotin S., Elle O.J. _Utilisation de la reconstruction stéréo-laparosocpique de la surface du foie pour compenser la déformation du pneumopéritoine par la modélisation biomécanique._ 2020 Conference d’humain physiologique virtuel (VPH), pp. 1-2, 2020 [Lien d'archive](https://hal.inria.fr/hal-03130613/document)

4. Nikolaev S., Peterlik I., Cotin S. _Correction stochastique des conditions aux limites pendant la chirurgie hépatique._ 2018 Symposium sur la couleur et l’informatique visuelle (CVCS), IEEE, pp. 1-4, 2018 [Lien de journal](https://ieeexplore.ieee.org/document/8496720) [Lien d'archive](https://hal.inria.fr/hal-01823810/document)

---

## Modélisation des strates de tissus mous communicatifs et de l’implant polymère

Je suis diplômé de l’Université d’État de Saint-Pétersbourg. Dans mon travail de master et les recherches suivantes, j’ai décrit la procédure qui simule l’expansion des implants ou des extenseurs dans les tissus mous en cas de chirurgie mammaire. L'idée de ce projet était de développer une prédiction visuelle de la forme de corps postopératoire, permettant aux chirurgiens d'avoir une vision claire pour des besoins du patient. En cas de chirurgie par lambeau, il se permet également d'estimer le volume de la solution physiologique requis pour l'extenseur ainsi que la forme d'un lambeau a cultivé pour la transplantation.

Le comportement des tissus mous a été modélisé par [un système de masse-ressort](https://fr.wikipedia.org/wiki/Syst%C3%A8me_masse-ressort) multicouche, non linéaire et anisotrope. Ce modèle est une rapidité d'exécution, mais reliée toujours sur les propriétés biomécaniques des tissus. Les tailles et les volumes des implants ont été pris des catalogues disponibles, et le profil asymétrique a été généré à l'aide d'une approche appelée [déformation de formes libres](http://alexianeb.free.fr/ProjetsDess/Techno/FFD.htm).

Selon l'implant utilisé, les résultats ont indiqué une similarité générale des reliefs avec des données réelles. Cependant, dans la plupart des cas, le rendu visuel n'était pas optimal, probablement à cause de la nature complexe sur des propriétés tissulaires qui doivent être intégrées dans le système.

### Publications

1. Nikolaev S.N. _Mise en oeuvre de l’interaction entre les tissus mous et les corps étrangers en utilisant le modèle modifié de voxel._ Journal d’outils informatiques en éducation, №. 3, pp. 28-32, 2013 [Lien de journal](http://ipo.spb.ru/journal/index.php?article/1581/) [Lien d'archive(Version anglaise)](http://arxiv.org/pdf/1403.7987.pdf)

2. Nikolaev S.N. _Système masse-ressort non linéaire pour la modélisation de grandes déformations des tissus mous._ Journal scientifique et technique des technologies de l’information, de la mécanique et de l’optique, №. 5 (87), pp. 88-94, 2013 [Lien de journal](https://ntv.ifmo.ru/ru/article/4322/article_4322.htm) [Lien d'archive(Version anglaise)](http://arxiv.org/pdf/1403.2294.pdf)

3. Nikolaev S.N. _Module de modélisation tridimensionnelle de l’augmentation mammaire en chirurgie._ Journal d’outils informatiques en éducation, №. 3, pp. 38-46, 2012 [Lien de journal](http://ipo.spb.ru/journal/index.php?article/1466/)

4. Adamskaia I.L, Vishnevskii A.A., Moroz V.Iu., Antipov I.G., Petrov A.G., Nikolaev S.N. _Biomodelage avec ordinateur en chirurgie reconstructive du sein._ Annales de chirurgie plastique, reconstructive et esthétique, №.  2, pp. 44-48, 2011 [~~Lien de journal~~ Lien de bibliothèque](http://elib.fesmu.ru/Article.aspx?id=239351)

---

[Retour]({{< ref "research/index.md" >}})

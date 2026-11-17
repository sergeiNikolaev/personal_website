---
title: "Research"
description: "A description of my research work."
featured_image: '/images/mars_style.jpg'
menu:
  main:
    weight: 4
---

## Embryo development investigation

As a postdoctoral researcher, I participated in a project related to the investigation of an embryo development process. The main idea of the work is to try to understand better how a fertilized egg develops in a complex biological organism. For the study, [acsidiacea](https://en.wikipedia.org/wiki/Ascidiacea) embryos were used because their development process has a simple structure. The shape of the embryo in space was described using a spherical [weighted Voronoi diagram](https://en.wikipedia.org/wiki/Weighted_Voronoi_diagram). Such a diagram approximates the shape with sufficient accuracy, but has a small number of parameters (five parameters for a cell) to describe it. Therefore, the complexity of the model is decreased. To present the development process, the Voronoi parameters were combined in multidimensional trajectories, which were studied and visualized using dimensional reduction techniques. Then a neural network was trained to predict the trajectory of a new embryo. However, the results show that further analysis and investigation are needed.

---

## Boundary conditions estimation to improve the simulation accuracy

I have successfully [written](https://theses.hal.science/tel-03416443) and [defended](https://www.youtube.com/watch?v=SYzDmdZIWF0) a PhD thesis. My thesis was a part of the grand project, the main idea of which is to create a navigation system for liver surgery. The main purpose of my work is to estimate the boundary conditions of the liver tissue for improving its simulation accuracy. Boundary conditions play an essential role in forming the predictive capacity of the model. But, in case of the liver, are presented mainly by ligaments, blood vessels, and surrounding organs, the properties of which are "patient specific" and can’t be measured reliably. Therefore, the main idea is to present the boundary conditions as a nonlinear [mass-spring system](https://en.wikipedia.org/wiki/Mass-spring-damper_model) and estimate its parameters.

Firstly, a generalized initial approximation is created. The ligaments positions are obtained with a statistical atlas. It is constructed from a set of models with segmented ligaments using a [large deformation diffeomorphic metric mapping method](https://www.sciencedirect.com/science/article/abs/pii/S1053811914005205?via%3Dihub), which is available in [deformetrica software](https://www.deformetrica.org). The ligament parameters are obtained from the constitutive law available in the literature and using a [parameter optimization module](https://help.febio.org/docs/FEBioUser-4-1/UM41-Chapter-7.html) from [FEBio software](https://febio.org).

The second step is estimation of spring parameters based on data from ligament model deformations computed in FEBio. And, after that, the correction of the whole system (liver model and ligaments as attached springs) is performed, taking the data obtained from a modality during surgery. For both procedures (parameters estimation and correction), a nonlinear [Kalman filtering approach](https://en.wikipedia.org/wiki/Kalman_filter) is applied, available in [Optimus plugin](https://github.com/sofa-framework/Optimus) from the [SOFA framework](https://www.sofa-framework.org).

To assess the proposed approach, several experiments were performed for both synthetic and real-data scenarios. The results show a certain improvement in simulation accuracy for the simulations with estimated boundary conditions.

#### Thesis reference:

Nikolaev S. _Identification and characterization of boundary conditions for patient specific biomechanical simulation_, 2021 [Thesis paper](https://theses.hal.science/tel-03416443) [Defense presentation](https://www.youtube.com/watch?v=SYzDmdZIWF0)&ensp;&ensp;&ensp;&ensp;&ensp;[Optimus plugin](https://github.com/sofa-framework/Optimus)

### Publications

1. Nikolaev S., Cotin S. _Estimation of boundary conditions for patient-specific liver simulation during augmented surgery._ International Journal of Computer Assisted Radiology and Surgery, Vol. 15, №. 7, pp. 1107-1115, 2020 [Journal link](https://link.springer.com/article/10.1007/s11548-020-02188-x) [Archive link](https://hal.archives-ouvertes.fr/hal-02634875/document) [Presentation link](https://www.youtube.com/watch?v=dztaapzOQqQ)

2. Mendizabal A., Tagliabue E., Hoellinger T., Brunet J.-N., Nikolaev S., Cotin S. _Data-driven simulation for augmented surgery._ In: Development and Novel Approaches in Biomechanics and Metamaterials, Chap. 5, pp. 71-96, 2020 [Journal link](https://link.springer.com/chapter/10.1007/978-3-030-50464-9_5) [Archive link](https://hal.inria.fr/hal-02538101/document)

3. Teaniti A., Brunet J.-N., Nikolaev S., Wang C., Edwin B., Cotin S., Elle O.J. _Use of stereo-laparoscopic liver surface reconstruction to compensate for pneumoperitoneum deformation through biomechanical modeling._ 2020 Virtual Physiological Human Conference (VPH), pp. 1-2, 2020 [Archive link](https://hal.inria.fr/hal-03130613/document)

4. Nikolaev S., Peterlik I., Cotin S. _Stochastic Correction of Boundary Conditions during Liver Surgery._ 2018 Colour and Visual Computing Symposium (CVCS), IEEE, pp. 1-4, 2018 [Journal link](https://ieeexplore.ieee.org/document/8496720) [Archive link](https://hal.inria.fr/hal-01823810/document)

---

## Interconnected soft tissue layers and polymeric implants modeling

I have graduated from the Saint Petersburg State University, where my diploma thesis and following research was focused on simulating the implant or expander placement and extension under soft tissues in case of breast surgery. The concept was to provide a visual prediction of the final body shape, thereby helping surgeons to specify patient needs more clearly. For flap surgery, it also allows estimating the volume of required saline for expanders as well as the form of grown tissue for transplantation.

The behavior of soft tissues was modeled with a multilayer, nonlinear, and anisotropic [mass-spring system](https://en.wikipedia.org/wiki/Mass-spring-damper_model). It is computationally efficient, while still relies on their biomechanical properties. The sizes and volumes of implants were taken from the available catalogs, and their asymmetric shape was obtained through a [free-form deformation approach](https://en.wikipedia.org/wiki/Free-form_deformation).

Depending on the used implant, the results indicated the general similarity in shape with real-world data. However, in most cases, the visual appeal was lacking, likely due to the complex nature of tissue properties that have to be provided.

### Publications

1. Nikolaev S.N. _Implementation of interaction between soft tissues and foreign bodies using modified voxel model._ Computer tools in education journal, №. 3, pp. 28-32, 2013 [Journal link](http://ipo.spb.ru/journal/index.php?article/1581/) [Archive link(English version)](http://arxiv.org/pdf/1403.7987.pdf)

2. Nikolaev S.N. _Non-linear mass-spring system for large soft tissue deformations modeling._ Scientific and technical journal of information technologies, mechanics and optics, №. 5 (87), pp. 88-94, 2013 [Journal link](https://ntv.ifmo.ru/ru/article/4322/article_4322.htm) [Archive link(English version)](http://arxiv.org/pdf/1403.2294.pdf)

3. Nikolaev S.N. _Module for three-dimensional modeling of breast augmentation in surgery._ Computer tools in education journal, №. 3, pp. 38-46, 2012 [Journal link](http://ipo.spb.ru/journal/index.php?article/1466/)

4. Adamskaia I.L, Vishnevskii A.A., Moroz V.Iu., Antipov I.G., Petrov A.G., Nikolaev S.N. _Biomodeling with computer in reconstructive breast surgery._ Annals of plastic, reconstructive and aesthetic surgery, №. 2, pp. 44-48, 2011 [~~Journal link~~ Library link](http://elib.fesmu.ru/Article.aspx?id=239351)

---

[Back]({{< ref "research/index.md" >}})

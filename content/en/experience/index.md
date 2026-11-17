---
title: "Experience"
description: "A description of my professional experience."
featured_image: '/images/mountain_style.jpg'
menu:
  main:
    weight: 3
---

Here is the description of my past working experience:

---

#### April 2022 - November 2023: Postdoctoral researcher in computational biology, University of Montpellier, Montpellier, France
- Objectives:
    + better understand how a single cell (fertilized egg) can develop into a complex biological organism
    + simulate embryo morphology, mainly shape, based on available embryo data and historical description of cells development
- Results:
    + represented embryo cells shape as parameters of a spherical weighted Voronoi diagram
    + ported from MATLAB to Python an optimization module, which extracts diagram parameters from available images, to execute the computation without license restrictions on the Jean Zay supercomputer
    + added peanut-shape cells processing and improved initialization of optimization parameters to construct the spherical weighted Voronoi diagram more accurately
    + implemented a software system to process and store in a Neo4j graph database the computed diagrams parameters and biological markers of cells
    + described the evolution of Voronoi diagram parameters during the development process and for different embryos as multidimensional trajectories in space
    + created a neural network using Transtab software to predict the dynamics of cells shape together with their division probability from a development history of the cells and constructed trajectories, the results show a possibility to predict the probability of cell division with an accuracy of 82%
- skills:
    + Computational biology, Morphology, Voronoi diagrams, Image processing, Machine learning, Graph databases
- technologies:
    + Python, NumPy, SciPy, Scikit-image, Matplotlib, Miniconda, Pandas, TensorFlow, Transtab, PyCharm, MATLAB, Neo4j, Cypher, Ubuntu Linux, Bash, Git

---

#### May 2017 - September 2021: PhD student, Research engineer, INRIA, University of Strasbourg, Strasbourg, France
- Objectives:
    + estimate liver’s boundary conditions to improve the simulation accuracy in an augmented reality system created for the surgery
    + simulate a realistic liver behavior as well as an influence of the surrounding organs and tissues in real time
- Results:
    + constructed a hyperelastic finite element method for liver deformations and a cubic spring system for boundary conditions
    + developed a component describing springs with polynomial stress strain relation, which was integrated into SOFA framework
    + participated in a software module implementation that allows estimating various model parameters using nonlinear Kalman filters
    + employed an approach based on a reduced-order unscented Kalman filter as the best choice for real-time performance/accuracy trade off
    + segmented and extracted markers from RGB-D image sequence to obtain observations for estimation process
    + carried out an optimization based on a preconditioner to improve the performance of the estimation process (computation time is 26% less)
    + created an approach based on deformable registration of liver shapes (large deformation diffeomorphic metric mapping) to obtain statistics for ligament positions
    + performed experiments based on synthetic (error is 66% less) and real (error is 23% less) data to show the improvement in accuracy for simulations with estimated boundary conditions
- skills:
    + Augmented reality, Numerical simulation, Finite element method, Mass-spring system, Kalman filters, Diffeomorphic metric mapping
- technologies:
    + C++, STL, Eigen, OpenCV, PCL, SOFA, FEBio, Qt, CMake, QtCreator, Python, NumPy, Matplotlib, Deformetrica, Ubuntu Linux, Bash, Git

---

#### May 2014 - November 2016: Software and research engineer, Scientific-Production Affiliate Energiya, Factory Energiya, Saint Petersburg, Russia
- Objectives:
    + create modules to find various signals in the radio waves spectrum, maintain a database to store the elements detected in records, collect statistics about characteristics of signals with an analyzing tool
- Results:
    + employed a software module that analyzes noise-like signal appearance and collects their basic information
    + ported from MATLAB to C++ a module that searches for frequency-hopping spread spectrum signals and extracts their basic parameters
    + created a component that puts information about detected signals and their parameters to a PostgreSQL database
    + developed a graphical user interface to show the spectrum frequency/sweep and indicate signals location
- skills:
    + Digital signal processing, Fourier analysis, FFT
- technologies:
    + C++, Intel IPP, STL, Boost, Qt, CMake, Visual Studio, SQL, PostgreSQL, MATLAB, MS Windows, Git

---

#### August 2010 - February 2014: Software engineer, OOO Bodynova, Saint Petersburg, Russia
- Objectives:
    + create a server-client software complex to model a patient body shape and results of implant and expander surgery procedures
    + simulate the biomechanical properties of skin, adipose, muscles, bones, and implants realistically
- Results:
    + developed software that simulates implant placement under soft tissues, estimated its accuracy and computation time
    + created a graphical user interface for the simulation software that allows selecting an implant from a catalogue and choosing its placement parameters
    + constructed an innovative multilayer, nonlinear, and anisotropic mass-spring system to describe soft tissues deformation, implemented as a C++ software unit
    + carried out an OpenGL based rendering component to observe a mass-spring system behavior
    + proposed and employed a modification of a voxel model to accelerate the processing of collision between implants and soft tissues
- skills:
    + Virtual reality, Numerical simulation, Mass-spring system, Image processing, Computational geometry, 3D computer graphics
- technologies:
    + C++, STL, WildMagic, WxWidgets, OpenCV, Bullet physics engine, OpenGL, OGRE, Visual Studio, HTML/CSS, JavaScript, Wolfram Mathematica, MS Windows, SVN

---

#### July 2008 - July 2010: Intern, Associate software engineer, EMC corporation, Saint Petersburg, Russia
- Objectives:
    + participate in a new storage system (driver) development
- Results:
    + developed low-level driver components for the data storage system, including a direct access disk mechanism (Bypass I/O) and a module for saving data cache in case of emergency shut off
    + configured hardware of four storage systems for remote access connections
- skills:
    + Storage device drivers, Linux development
- technologies:
    + C, gdb, make, Valgrind, Linux utils, Vim, Perl, Linux, SVN

---

[Back]({{< ref "experience/index.md" >}})

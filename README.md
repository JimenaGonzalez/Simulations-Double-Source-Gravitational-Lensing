# Simulations of Double-Source Plane Gravitational Lensing

## Objective of this project:
Producing realistic simulations of double-source plane lensing systems. Then, these simulated images are going to be used to train a convolution neural network (CNN) to find these kind of systems in real data.


## Definiton:
**Double-source plane lensing systems** are systems in which there are two galaxy sources sufficiently align behind a heavy galaxy that curves their light. The lensing of the light of each source produces multiple images of them on the sky that can be perceived as two Einstein rings. 

## Description of the project and the repository

To generate these simulations we are using the **Lenstronomy** package: Here is the [Documentation](https://lenstronomy.readthedocs.io/en/stable/).

In the beginning, we were planning on simulating the whole system using lenstronomy. Since we want to create simulations that are as most realistic as possible, we needed to take into account the correlation there is between 3 galaxy properties: apparent magnitude, size, and velocity of dispersion. This correlation is described by the **Fundamental Plane** relation, and the **Faber-Jackson** relation. In this [notebook](https://github.com/JimenaGonzalez/Simulations-Double-Source-Gravitational-Lensing/blob/master/Faber-Jackson%20Relation.ipynb), you will find a comparison of the Faber-Jackson fit found by [D’Onofrio, Cariddi, et al](https://iopscience.iop.org/article/10.3847/1538-4357/aa6540/pdf) with a SLAC sample. In this [notebook](https://github.com/JimenaGonzalez/Simulations-Double-Source-Gravitational-Lensing/blob/master/Fundamental%20Plane%20Relations.ipynb) you will find an implementation of the functions that calculate the apparent magnitude and the angular diameter of an elliptical galaxy given its velocity of dispersion. In that notebook you will also find a comparison between the fit found by [Hyde and Bernardi](https://arxiv.org/pdf/0810.4924.pdf) and the same SLAC sample used in the previous notebook.

![Alt Text](Animacion.gif)

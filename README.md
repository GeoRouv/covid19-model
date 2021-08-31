# covid-compartmental-model
📈 Examine the impact of COVID-19 spread by using a custom epidemiological model.

<img src="./intro_image.jpg" alt="drawing" width="800"/>

## Requirements

- [Copasi](http://copasi.org/)  
- [Jupyter](https://jupyter.org/) (or any notebook editor)


## Methods

Simulation and modeling is becoming a standard approach to understand complex bio-
chemical processes. Therefore, there is a big need for software tools that allow access to
diverse simulation and modeling methods as well as support for the usage of these method.
COPASI is an open-source software application for creating and solving mathematical
models of biological processes such as metabolic networks, cell-signaling pathways, reg-
ulatory networks, infectious diseases, and many others. In this case, this software was
utilized as an epidemic simulator since the the biochemical reactions networks resemble
the viruses behaviour.

As an extra step, the same model without the vaccination part, was implemented in
python (*see SIERD_model*) for this project as well.

## Model

The basic SEIR model is expanded to six compartments to simulate the epidemic of
COVID-19. Six state variables are considered within a population, that is, S(t), E(t),
I(t), R(t), D(t), and V(t), denoting the number of susceptible, exposed (infected, but not
yet infectious), infectious (symptomatic and asymptomatic), recovered, dead, and vacci-
nated cases, respectively. Thus, the human population is denoted by N(t) = S(t)+E(t)+
I(t) + R(t) + D(t) + V (t).

<img src="./model.jpg" alt="drawing" width="500"/>

## Differential equations

The model culminates to a six-dimensional system of ordinary differential equations as
follows.



## Copasi Guideline:

- Import *SIERD-V.cps* into COPASI

- To run the model for the initial parameters, go to 'Tasks>Time Course', create a plot by pressing the button 'Output Assistant' and hit 'Run'.

- To apply Sensitivity Analysis, head over to 'Tasks > Parameter Scan', press 'Create' and choose a global quantity. Then, you are ready to to apply sensitivity analysis by pressing 'Run'.

Change parameters to your liking


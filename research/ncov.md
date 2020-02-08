---
layout: default
title: 2019 nCoV
parent: Research
nav_order: 2
---

# 2019 nCoV

I also enjoy exploring and visualizing public datasets. For example, the recent outbreak of the novel coronavirus 2019 nCoV caught my attention. Here is a bar chart showing the growth in the number of confirmed cases in China, separated by Province:

![](/assets/images/ncov1.png){:width="900px"}

Clearly, Hubei Province has by far highest number of cases, but do the other provinces show qualitatively similar behavior? To visualize the growth pattern, here are simple line plots with a linear (top) and logarithmic scale (lower) for the y-axis:
![](/assets/images/ncov2.png){:width="900px"}

Indeed, they all seem to behave similarly. It could be useful to have a model describing this behavior, so let's start by making the following assumptions:

<!-- Using this: https://alexanderrodin.com/github-latex-markdown/ -->

1. The number of cases can be described by a power law of the form ![y = \alpha x^{\beta} + \gamma](https://render.githubusercontent.com/render/math?math=y%20%3D%20%5Calpha%20x%5E%7B%5Cbeta%7D%20%2B%20%5Cgamma)

2. Poisson counting statistics, i.e. the uncertainty of each data point is as the square root

To check if the assumption of a power law makes sense, let's start by modeling the data from Hubei Province. The model has three parameters (![\alpha, \beta, \gamma](https://render.githubusercontent.com/render/math?math=%5Calpha%2C%20%5Cbeta%2C%20%5Cgamma)
), which we can estimate using Bayesian inference.

We can efficiently sample the posterior distributions of the model parameters using [pymc3](https://docs.pymc.io/):
![](/assets/images/ncov3.png){:width="900px"}

Looks like a power law is a pretty good fit! Here is the joint posterior distribution:
![](/assets/images/ncov4.png){:width="900px"}

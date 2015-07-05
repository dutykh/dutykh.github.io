---
layout: post
title: Thin film dynamics
---

I am getting also interested in the dynamics of thin films which flow down the vertical wall. There are many differences with the classical water wave models, besides flipping the wave propagation direction (**horizontal** to **vertical**). For instance, the viscosity plays a very important role in thin films, while it is negligible in water wave modelling. Another point is the surface tension force which has to be taken into account in the model. Below we show a numerical simulation of the instability development from a periodic perturbation (*please, don't hesitate to open to the full screen*):

<iframe width="480" height="360" src="http://www.youtube.com/embed/jkZ96ZmNAns" frameborder="0"> </iframe>

We solve the so-called Shkadov's model (also known as the viscid Saint-Venant equations) in a periodic domain using the finite volume method (Rusanov flux is used). The dispersive term is discretized using the central finite differences. The semi-discrete model is solved in time with an adaptive Runge-Kutta scheme.

A research direction to be continued!

---
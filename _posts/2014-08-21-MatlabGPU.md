---
layout: post
title: Matlab + GPU
---

In order to warm up before the Fall 2014, I decided to test Matlab GPU computing capabilities on my laptop which is equiped with the [GeForce GTX 680M](http://www.geforce.com/hardware/notebook-gpus/geforce-gtx-680m) graphics card.

In order to take the full advantage of this hardware, the algorithm has to be suitable for the extreme parallelisation. That is why the choice of pseudo-spectral codes was natural. I have to say that porting of an existent Matlab (CPU) code to GPU is relatively easy.

Here you can see two simulations of the 2D incompressible [Navier-Stokes](http://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_equations) and [Charney-Hasegawa-Mima](http://en.wikipedia.org/wiki/Hasegawa%E2%80%93Mima_equation) (CHM) equations. A random distribution of the vorticity was taken as the initial condition. No forcing. No dissipation in CHM. Just freely decaying turbulence. The resolution is 512x512 in both cases.

* Navier-Stokes simulation (Re = 10 000):

<iframe width="420" height="315" src="//www.youtube.com/embed/rKQ5nUTJKjU" frameborder="0"></iframe>

* CHM simulation:

<iframe width="420" height="315" src="//www.youtube.com/embed/BP4VhEKSDF4" frameborder="0"></iframe>

Now one can ask the legitimate question about the observed speed-ups. In my case (on the resolutions reported above) I observed the speed-up from 2 to 3 times. For higher resolutions this number is expected to increase. Note however, that the resolution is limited by the available GPU memory (~3.9 Gb for the GPU I have).

This modest speed-up can be explained by the following reasons:

* the GPU code is not yet fully optimized
* the gain in speed is annihilated by the cost of memory transfer to/from GPU

The profiling results seem to favour the latter explanation.

---
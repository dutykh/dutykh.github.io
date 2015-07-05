---
layout: post
title: sine-Gordon equation
---

Thanks to my collaborator from [Rouen](http://en.wikipedia.org/wiki/Rouen) (France) - [Jean-Guy Caputo](http://lmi.insa-rouen.fr/membres/20-caputo.html) I discovered many interesting features of the [sine-Gordon](http://en.wikipedia.org/wiki/Sine%E2%80%93Gordon_equation) equation. In particular, he invited me to study the dynamics of some special solutions (*kinks* and *breathers*) in tree-like geometries.

For the sake of illustration, here is a simulation of a kink passing through a T-junction, since it possesses enough energy to do it:

<iframe width="480" height="360" src="http://www.youtube.com/embed/2pLqAKOrZHU" frameborder="0"> </iframe>

And another kink which has a *sub-critical* velocity. Thus, it cannot pass through the junction:

<iframe width="480" height="360" src="http://www.youtube.com/embed/Uz3gWlkg8_g" frameborder="0"> </iframe>

More details on the obtained results can be found in our first common preprint:

* J.-G. Caputo & **D. Dutykh**. [Nonlinear waves in networks: a simple approach using the sine-Gordon equation](http://hal.archives-ouvertes.fr/hal-00951705/). Submitted, 2014

Moreover, I just released in Open source the script for [FreeFem++](http://www.freefem.org/ff++/) that we used to perform the simulations shown above:

* [https://github.com/dutykh/sineGordon_FreeFem](https://github.com/dutykh/sineGordon_FreeFem/)

**Any comments are welcome!**

---
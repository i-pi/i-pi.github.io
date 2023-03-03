---
layout: page
title: "The Socket Interface"
subheadline: ""
teaser: "Run i-PI and the force calculator over different HPC centers!"
permalink: "/about/interface/"
header:
   image_fullwidth: "wpig6_blue.jpg"
---

Although the modular design of the code allows for direct, library-like
calls to force evaluators, the main mode of functioning of i-PI allows
to use a separate ab initio or empirical force evaluation code to
compute interatomic forces.
The implementation is based on a client-server paradigm, where i-PI
acts as the server and deals with the propagation of the nuclear
dynamics, whereas the calculation of the potential energy, forces and
the potential energy part of the pressure virial is delegated to one
or more instances of an external code, acting as clients. 

i-PI was originally designed to perform ab initio PIMD - where the cost of the
force evaluation is overwhelming relative to the ionic dynamics.
However, it has since grown to do much more than that.
The implementation of i-PI is efficient enough that it can be used with empirical
forcefields and machine-learned potentials without incurring a large overhead.
If you experience very large overheads, please contact the developers! It is 
likely that some easy solutions are possible. See more about i-PI implementation in the publication
that accompanies its release.

![socket-interface scheme](/images/ipi-interface-scheme.png)

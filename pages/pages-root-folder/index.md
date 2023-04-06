---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: page
title: 
header:
  image_fullwidth: wpig6_blue.jpg

#callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
#
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---


i-PI is a universal force engine interface
written in Python, designed to be used together with an ab-initio, machine-learned,
or force-field based evaluation of the interactions between the atoms. 
The main goal is to
decouple the problem of evolving the ionic positions to sample the
appropriate thermodynamic ensemble and the problem of computing the
inter-atomic forces.

<p align="center">
  <img src="{{ site.urlimg }}ipi-logo-alpha.png" alt="iPi-logo" />
</p>

The implementation is based on a client-server paradigm, where i-PI
acts as the server and deals with the propagation of the nuclear
motion, whereas the calculation of the potential energy, forces and
the potential energy part of the pressure virial is delegated to one
or more instances of an external code, acting as clients. Other types
of electronic-structure information can also be communicated for
performing advanced types of dynamics.

i-PI is free software, distributed under a dual MIT/GPLv3 licence. You
are welcome to dowload, use, modify and redistribute it. 
To get the most up-to-date version, fetch it from the 
[official i-PI repo](https://github.com/i-pi/i-pi). If you find it
useful for your research, please cite us:

[Kapil et al., Comp. Phys. Comm. 236, 214--223 (2018)](https://doi.org/10.1016/j.cpc.2018.09.020)


As of today, the following electronic-structure codes provide out-of-the-box an i-PI interface: 
[CP2K](https://www.cp2k.org/), 
[DFTB+](http://www.dftb-plus.info/), 
[LAMMPS](http://lammps.sandia.gov/), 
[Quantum ESPRESSO](http://quantum-espresso.org), 
[Siesta](http://departments.icmab.es/leem/siesta/), 
[FHI-aims](https://aimsclub.fhi-berlin.mpg.de/), 
[Yaff](http://molmod.github.io/yaff/), 
[deMonNano](http://demon-nano.ups-tlse.fr/), 
[plumed](http://www.plumed.org/), 
[ASE](https://wiki.fysik.dtu.dk/ase/),
[TBE](https://www.questaal.org/),
[CASTEP](http://castep.org/).
[AMS](https://www.scm.com/doc/plams/examples/i-PI-AMS.html).
If you know a code that is missing in this list, please contact the developers. If you are interested in interfacing your code to i-PI please get in touch,
we are always glad to help! 

A few machine-learning potentials are also interfaced with i-PI, such as 
[n2p2](https://github.com/CompPhysVienna/n2p2) (interface through LAMMPS),
[sGDML](http://www.sgdml.org/),
[AMS](https://www.scm.com/doc/plams/examples/i-PI-AMS.html),
and others.

If you have questions about running i-PI calculations, or including new features
into the code, you can get help on the [user forum](https://groups.google.com/forum/#!forum/ipi-users), 
or on the [github pages](https://github.com/i-pi/i-pi).

---
title: "G-ADOPT"
type: page
weight: 10
category: software
thumbnail: "/images/research/gadopt.png"
description: "A computational platform for geoscientific simulations and adjoint-based inversion, built on Firedrake."
---

<div class="research-hero">
    <img src="/images/research/gadopt.png" alt="G-ADOPT logo">
</div>

[G-ADOPT](https://gadopt.org/) (Geoscientific ADjoint Optimisation PlaTform) is our flagship computational platform for simulating geoscientific flows and solving inverse problems. Built on top of [Firedrake](https://www.firedrakeproject.org/), it lets researchers write simulation code in Python that closely mirrors the underlying mathematics, while Firedrake handles the automatic generation of efficient finite element code and the derivation of discrete adjoint models via [dolfin-adjoint](http://www.dolfin-adjoint.org/en/latest/).

G-ADOPT supports a range of physical approximations — from incompressible Boussinesq convection through to compressible anelastic formulations and viscoelastic Maxwell rheology for GIA — across 2D and 3D geometries, including full spherical shells. It couples Stokes and energy solvers with time-stepping schemes (explicit and implicit Runge-Kutta via Irksome), multi-material level-set methods, and PDE-constrained optimisation through the Rapid Optimisation Library (ROL). The platform runs at scale on national HPC facilities like NCI's Gadi supercomputer.

G-ADOPT is funded by the Australian Research Data Commons, AuScope, and the Australian Research Council, among others, and is developed in collaboration with Imperial College London and the University of Sydney.

**Source:** [github.com/g-adopt/g-adopt](https://github.com/g-adopt/g-adopt)

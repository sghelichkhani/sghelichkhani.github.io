---
title: "Mantle Convection"
type: page
weight: 1
category: research
thumbnail: "/images/research/mantle-convection.png"
description: "Adjoint-based inversion for reconstructing Earth's thermal and chemical evolution through deep time."
---

<div class="research-hero">
    <img src="/images/research/mantle-convection.png" alt="Global mantle convection simulation showing thermal anomalies">
</div>

The Earth's mantle convects over geological timescales, driving plate tectonics, volcanism, and the long-term thermal and chemical evolution of the planet. One of the grand challenges in geodynamics is reconstructing this evolution — building a "digital twin" of Earth's mantle that is consistent with the observational record we have today, including seismic tomography, surface heat flow, dynamic topography, and the geoid.

My work in this area focuses on adjoint-based inversion methods that allow us to run mantle convection simulations backward and forward in time, optimising unknown initial conditions (and other parameters) so that the resulting model matches present-day observations. This involves solving large-scale, non-linear, time-dependent inverse problems on spherical shell geometries using the finite element method.

A key result of this effort is the development of automatic adjoint capabilities within [G-ADOPT](/research/g-adopt/), which removes the need for hand-derived adjoint equations and makes it practical to tackle increasingly realistic Earth models with complex rheologies. By leveraging the algorithmic differentiation capabilities built into [Firedrake](https://www.firedrakeproject.org/) and [dolfin-adjoint](http://www.dolfin-adjoint.org/en/latest/), we can differentiate through entire time-dependent simulations to compute gradients of observational misfits with respect to initial conditions, boundary conditions, and material parameters — all without writing a single line of adjoint code by hand.

This work opens the door to systematically exploring questions about the initial thermal state of the mantle, the history of plate motions, and the role of compositional heterogeneity in shaping the structures we image seismically today.

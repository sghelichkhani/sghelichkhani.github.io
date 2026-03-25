---
title: "gtrack"
type: page
weight: 14
category: software
thumbnail: "/images/research/gtrack-placeholder.png"
description: "Lagrangian particle tracking for computing lithospheric structure through geological time using plate reconstructions."
---

<div class="research-hero">
    <img src="/images/research/gtrack-placeholder.png" alt="gtrack">
</div>

[gtrack](https://gtrack.gadopt.org/) computes lithospheric structure through geological time using plate tectonic reconstructions. It provides the kinematic boundary conditions that feed into [G-ADOPT](/research/g-adopt/) mantle convection simulations, bridging the gap between plate tectonic data and geodynamic modelling.

The package has two main capabilities. First, it tracks seafloor ages by advecting Lagrangian particles from mid-ocean ridges through time using stage rotation poles, detecting subduction zone collisions via velocity-based criteria, and translating ages into lithospheric thickness through thermal models like half-space cooling. Second, it rotates user-provided points representing continental lithospheric structure (for example from seismic tomography) backward through geological time to reconstruct past configurations.

Both workflows produce point clouds in Cartesian coordinates that are directly compatible with G-ADOPT's spatial interpolation system. Under the hood, gtrack delegates the computationally intensive plate reconstruction operations to [pygplates](https://www.gplates.org/docs/pygplates/), the C++ backend of GPlates, using batched plate operations for significant speedups over per-point rotation. Results are validated against GPlately's reference implementation.

**Source:** [github.com/sghelichkhani/gtrack](https://github.com/sghelichkhani/gtrack)

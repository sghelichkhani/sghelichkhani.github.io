---
title: "Continental-Scale Groundwater"
type: page
weight: 3
category: research
thumbnail: "/images/research/groundwater.png"
description: "Adjoint methods for the Richards equation to build digital twins of continental aquifer systems."
---

<div class="research-hero">
    <img src="/images/research/groundwater.png" alt="Streamline plot of groundwater velocity field">
</div>

Groundwater is one of the most important and least understood components of the water cycle at continental scales. I am working on developing adjoint methods for the Richards equation — the nonlinear PDE governing variably saturated flow through porous media — to enable data-driven modelling of groundwater systems at the scale of entire continents.

The goal is to build digital twins of continental aquifer systems that can assimilate satellite observations (such as GRACE gravity data and InSAR surface deformation) to constrain subsurface properties and predict groundwater dynamics under changing climate and extraction scenarios. Getting this right requires solving a genuinely hard inverse problem: the Richards equation is nonlinear, the parameter space is enormous, and the observational constraints are sparse and indirect.

Our approach couples the adjoint capabilities of [G-ADOPT](/research/g-adopt/) with high-resolution mesh representations of continental geology and topography, running at scale on national HPC facilities. This work is funded through the SmartSat CRC and the ANU Institute for Water Futures.

---
title: "SRTS"
type: page
weight: 12
category: software
thumbnail: "/images/research/srts-placeholder.png"
description: "Tomographic resolution filtering for meaningful comparison between geodynamic models and seismic observations."
---

<div class="research-hero">
    <img src="/images/research/srts-placeholder.png" alt="SRTS placeholder">
</div>

[SRTS](https://github.com/g-adopt/srts) implements tomographic resolution filtering following the methodology of Ritsema et al. (2007). When comparing geodynamic model predictions against seismic tomography, it is essential to account for the fact that seismic imaging has limited and spatially variable resolution — a geodynamic model may contain structure that is real but unresolvable by seismology. SRTS applies the resolution operators from published tomography models (S12RTS, S20RTS, S40RTS) to any geodynamic field, producing a filtered version that represents what a seismologist would actually recover.

The package performs spherical harmonic expansion, depth reparameterisation onto a spline basis, and application of the resolution matrix, all in a fully vectorised Python implementation that improves on the precision of the original Fortran codes. It integrates naturally with G-ADOPT workflows for model-data comparison in mantle convection inversions.

**Source:** [github.com/g-adopt/srts](https://github.com/g-adopt/srts)

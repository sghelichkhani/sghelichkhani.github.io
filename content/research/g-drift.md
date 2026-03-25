---
title: "G-DRIFT"
type: page
weight: 11
category: software
thumbnail: "/images/research/gdrift.png"
description: "A FAIR-compliant data toolkit for geodynamic and seismological datasets used in mantle convection studies."
---

<div class="research-hero">
    <img src="/images/research/gdrift.png" alt="G-DRIFT logo">
</div>

[G-DRIFT](https://gdrift.gadopt.org/) (Geodynamics Data Reformatting and Integration Facilitation Toolkit) is the data backbone of the G-ADOPT ecosystem. It provides a unified, FAIR-compliant Python interface for loading and working with the geodynamic and seismological datasets that underpin mantle convection studies — things like 1D reference Earth models (PREM), solidus profiles, 3D seismic tomography models (25 published models, including S40RTS, SAVANI, and SEMUCB-WM1), thermodynamic lookup tables for mineral physics properties, and anelasticity correction models.

G-DRIFT handles automatic downloading, caching, and cryptographic verification of datasets from a central repository, and provides physics-aware interpolation (1D spline, 3D KD-tree with multiple kernels) for mapping between different model parameterisations. It solves a real problem: the datasets used in geodynamic inversions are typically scattered, poorly documented, and difficult to reproduce. G-DRIFT centralises them in one well-curated package.

**Source:** [github.com/g-adopt/g-drift](https://github.com/g-adopt/g-drift)

---
title: "LLNL-ToFi"
type: page
weight: 13
category: software
thumbnail: "/images/research/llnltofi-placeholder.png"
description: "Tomographic filtering using the LLNL-G3D-JPS resolution matrix for seismic velocity models."
---

<div class="research-hero">
    <img src="/images/research/llnltofi-placeholder.png" alt="LLNL-ToFi">
</div>

[LLNL-ToFi](https://github.com/g-adopt/llnltofi) applies the resolution matrix from the LLNL-G3D-JPS seismic tomography model (Simmons et al., 2015) to arbitrary velocity models through a single sparse matrix-vector multiplication. It is a modern Python reimplementation of the original Fortran-based LLNL_ToFi code by Bernhard Schuberth at LMU Munich.

The LLNL-G3D-JPS model provides a resolution matrix that encodes how the seismic imaging process smears and distorts the true Earth structure. By applying this operator to a geodynamic velocity model, we can produce a filtered prediction that is directly comparable to the published tomography — accounting for the uneven data coverage and regularisation inherent in seismic inversions.

The package operates on 44 depth layers spanning from the crust to the core-mantle boundary (over one million grid points), supports both geographic and Cartesian coordinate systems, and handles automatic downloading and caching of the resolution data. It also fixes a boundary indexing bug present in the original Fortran code that affected a small number of matrix entries.

Like [SRTS](/research/srts/), LLNL-ToFi integrates naturally with [G-ADOPT](/research/g-adopt/) workflows for quantitative model-data comparison in mantle convection inversions.

**Source:** [github.com/g-adopt/llnltofi](https://github.com/g-adopt/llnltofi)

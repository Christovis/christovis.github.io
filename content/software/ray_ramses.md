+++
title = "Ray-Ramses"
description = "Ray-tracing code for AMR CFD simulations"
weight = 1

[extra]
local_image = "preview_tng100_gas_vel.jpg"
github = "https://github.com/Christovis/ray-ramses"
tags = ["cosmology", "ray-tracing"]
+++

A open-source ray tracing code to compute integrated cosmological observables on the fly in AMR N-body simulations. Unlike conventional ray tracing techniques, our code takes full advantage of the time and spatial resolution attained by the N-body simulation by computing the integrals along the line of sight on a cell-by-cell basis through the AMR simulation grid. Moroever, since it runs on the fly in the N-body run, our code can produce maps of the desired observables without storing large (or any) amounts of data for post-processing. The ray tracing methodology presented here can be used in several cosmological analysis such as Sunyaev-Zel’dovich and integrated Sachs-Wolfe effect studies as well as modified gravity. Our code can also be used in cross-checks of the more conventional methods, which can be important in tests of theory systematics in preparation for upcoming large scale structure surveys.

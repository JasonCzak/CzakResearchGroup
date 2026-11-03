---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

Research in the Czak Research Group focuses on mathematical and computational approaches to complex physical systems. Current work spans nonlinear reaction–diffusion systems, pattern formation and control, numerical methods, spatiotemporal epidemic modeling, dendritic growth, and computational analysis of ecological systems.

## Reaction–diffusion systems and pattern formation

The Gray–Scott model uses two interacting model species, commonly denoted *u* and *v*, to generate many forms of spatiotemporal behavior. Depending on parameter choices, simulations can produce stationary pulses, traveling waves, self-replicating structures, coarsening behavior, and transient or sustained chaos. We use the model as a computational laboratory for studying how patterns emerge, evolve, and respond to changes in parameters and control protocols. Our simulations run on GPUs, which lets us explore large two-dimensional lattices and long run times.

<div class="sim-video-row">
  <figure class="sim-video">
    <video controls muted loop playsinline preload="metadata" poster="{{ base_path }}/images/gray-scott-chaos-2d-a-poster.jpg">
      <source src="{{ base_path }}/assets/videos/gray-scott-chaos-2d-a.mp4" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption>GPU-enabled Gray–Scott chaos-regime simulation in 2D.</figcaption>
  </figure>
  <figure class="sim-video">
    <video controls muted loop playsinline preload="metadata" poster="{{ base_path }}/images/gray-scott-chaos-2d-b-poster.jpg">
      <source src="{{ base_path }}/assets/videos/gray-scott-chaos-2d-b.mp4" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption>GPU-enabled Gray–Scott chaos-regime simulation in 2D.</figcaption>
  </figure>
</div>

## Localized pattern control

Control of chaos is usually applied to an entire system. We instead apply spatially localized perturbations, including parameter variation, electric-field effects, and time-delayed feedback, to a selected region and examine how the effects propagate through the surrounding nonlinear system. In the Gray–Scott model, localized time-delayed feedback creates stable periodic structures inside an otherwise chaotic state ([*Phys. Rev. E* 104, 064213, 2021]({{ base_path }}/publications/)).

<figure class="sim-video">
  <video controls muted loop playsinline preload="metadata" poster="{{ base_path }}/images/gray-scott-localized-control-2d-poster.jpg">
    <source src="{{ base_path }}/assets/videos/gray-scott-localized-control-2d.mp4" type="video/mp4">
    Your browser does not support HTML5 video.
  </video>
  <figcaption>GPU-enabled Gray–Scott chaos-regime simulation in 2D with localized control applied.</figcaption>
</figure>

## Spatially varying parameters

Most studies use parameters that are fixed throughout space. We investigate functional forms that vary important parameters across the lattice. Sinusoidal and other oscillatory functions can combine behaviors associated with several parameter regimes within one simulated system, producing new and intricate structures.

## Numerical reliability

The Euler method is simple and widely used, but simulation accuracy depends on the time step and on the behavior of the system. Our work with Owen Jones examines accuracy across distinct Gray–Scott regimes and near transitions between them, and finds that a numerically stable time step is not necessarily a reliable one: chaotic regimes can require a drastically smaller step to keep finite-time trajectories accurate. See [Publications]({{ base_path }}/publications/).

## Spatiotemporal epidemic modeling

Classical SIR models assume a well-mixed population. Our work extends the framework to a two-dimensional lattice with local interactions between neighboring regions. Finite-difference simulations reveal spatial epidemic waves and support extensions involving demographic effects, incubation periods (SEIR), and loss of immunity (SIRS).

## Emerging directions

- **Dendritic growth and modeling:** a developing project using computational modeling and numerical simulation to investigate dendritic growth and pattern formation.
- **Computational ecology and forest dynamics:** an open project using spatial ecological data, including tree-canopy data, to study structure and change in forest systems.
- **Machine learning for pattern classification:** classifying simulated patterns and predicting which patterns appear in unexplored regions of parameter space.

## Support and collaboration

- 4-VA Collaborative Research Grant, James Madison University and Virginia Tech (2025–ongoing), with Michel Pleimling

---
title: "Data-driven discovery of shared latent dynamics across sessions"
permalink: /projects/shared-latent-dynamics/
excerpt: "Data-driven discovery of nonlinear latent dynamics and aligned neural population activity across sessions."
tags:
  - neural-dynamics
  - latent-variable-models
  - fast-learning
  - decision-making
  - data-driven
  - behavior
header:
  teaser: dynest_small.png
---

<img align="left" src="../../images/dynest.png" alt="Probabilistic model to estimate latent neural trajectories and structure of latent dynamics from neural recordins across days. Dynamics are assumed to be shared across days but mapping from latents to single neural spiking is flexible across days." title="Data-driven estimation of shared latent dynamics." hspace=20px vspace=5px width="35%" />
Reliably estimating and interpreting neural population dynamics in complex tasks, to link neural circuits to the behavioral computations they support, faces two crucial challenges: (1) balancing model flexibility with interpretability and reducing solution degeneracy, and (2) overcoming the limitations of short recording sessions and drift in chronic recordings, in tasks with heterogeneous trials and multi-dimensional behavioral variability, and where matching trials or neurons across days is challenging. We developed a method that learns a __shared nonlinear, low-dimensional dynamical system__ across sessions that not only captures population co-variability through latent trajectories but learns correct dynamical solutions that enable forecasting. This allows combining or comparing trials across days in a shared latent space.

In collaboration with Christine Constantinople at NYU, we used this model to analyze recordings from orbitofrontal cortex (OFC) in rats performing a value-guided decision-making task. Joint optimization with a shared dynamical prior outperformed standard alignment methods, uncovering modulation of latent dynamics on single trials as well as across diverse conditions — time, belief states, stimuli, and decisions. Combining data across sessions allowed us to identify latent dynamics on different timescales: trial-by-trial updates of “belief states” during rare but diagnostic context switches,  as well as changes in neural “speeds” during deliberation within individual trials controlling decision timing. Our approach to __dynamics-based alignment across sessions__ using a well-conditioned yet flexible model offers the opportunity to study __richer behavioral variability and multiplexed computations__ in complex, or even more naturalistic, tasks, as well as __track neural representations across days__.
---
title: "Data-driven models for control of biomechanical bodies"
permalink: /projects/biomechanical-control-models/
excerpt: "Closed-loop neural controllers with biologically grounded sensory feedback for realistic locomotor behavior."
tags:
  - biomechanics
  - sensory-feedback
  - imitation-learning
  - behavior
header:
  teaser: biomech.png
---

<img align="left" src="../../images/biomech.png" alt="Neural network controller of biomechanical bodies simulated in physics engines, with realistic encoding of sensory feedback" title="" hspace=20px vspace=20px width="30%" />
Neuroscientists have long studied central pattern generators (CPGs) that generate oscillatory activity patterns for rhythmic motor outputs, such as for limbed locomotion. However, when a walking animal encounters an unexpected perturbation (e.g. uneven terrain, being pushed), it must integrate feedback from proprioceptive sensory neurons with ongoing rhythmic feedforward commands to adjust, recover, and sustain walking. I am using a data-driven integrative modeling approach to identify neural computations underlying robust locomotion in Drosophila (fruit fly model system) - modular neural network controllers, with biologically grounded models of proprioceptive sensing, controlling biomechanical models simulated with physics engines, and trained using imitation learning to produce realistic 3D kinematics. By manipulating the activity of proprioceptive neurons in silico and quantifying altered kinematics in these closed-loop models, I am able to identify the role of different classes of sensory feedback (joint positions, joint velocity, contact) in shaping walking behavior. In collaboration with John Tuthill at UW, I am also comparing these predictions to behavioral responses of actual walking flies to optogenetic activation of sensory neurons.
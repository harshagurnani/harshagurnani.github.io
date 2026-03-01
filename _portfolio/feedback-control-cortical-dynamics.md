---
title: "Feedback control of cortical dynamics"
order: 2
permalink: /projects/feedback-control-cortical-dynamics/
excerpt: "How feedback, intrinsic dynamics, and controllability shape dynamical constraints on fast learning."
tags:
  - sensory-feedback
  - recurrent-neural-networks
  - brain-computer-interfaces
  - theory
  - neural-dynamics
  - multi-region
  - motor-learning
header:
  teaser: bci_small.png
---

<img align="left" src="../../images/controlled.png" alt="Controlled dynamical system acting on downstream effector. Changes in the environment can be handled by feedback correction, changes in the control policy or changes to the dynamics." title="Learning in a controlled system." hspace=20px vspace=5px width="30%" />
I use _recurrent neural networks (RNNs)_ to model motor control tasks, including the use of motor BCI (brain-computer interfaces), where feedback about the output - either as _"efference copy"_ and/or _sensed state_ of the effector (limb, cursor, voice) - is a critical component to successful task completion. This feedback is needed to alter network dynamics in real time, in response to noise or external perturbations, to adjust the motor output. Moreover, learning in these networks may involve changes to the feedback inputs rather than to the recurrent network structure itself, especially when the dynamics are expressive enough. Borrowing insights from work on state-feedback controllers and modelling these "controllers" using neural network architectures, I study the implications of such an organization on __observed neural activity structure__ and __dynamical constraints on motor learning__.

<img align="left" src="../../images/constraint.png" alt="Dynamical constraints on learning. Controlled motor cortical activity can be adapted to use different BCI decoders, but the desired  trajectories are subject to dynamical, and not just geometric constraints. Image shows three sets of trajectories on a flowfield. One trajectory (T1) is along the flowfield and is easy, another trajectory (T2) is against the recurrent flowfield and requires large or infeasible inputs, and a third trajectory (T3) requires the neural state to firrst be pushed out in a less controllable direction in state space and is also difficult." title="Dynamical constraints on learning." hspace=20px vspace=5px width="60%" />
Previous work has shown that neural activity is often constrained to low-dimensional manifolds. We find that beyond neural geometry, structured dynamics on these manifolds further constrain learning on fast timescales. For motor circuits, these dynamics are shaped not just by internal recurrence but by low-dimensional control inputs based on continuous sensory feedback. By studying learning phenomena in a brain-computer interface (BCI) task and modelling plasticity at upstream controllers (such as cerebellar and premotor areas), we show that (i) feedback controllability, (ii) control bottlenecks, and (iii) input-driven flow-fields explain variable success and rates of adaptation to different BCI decoders, which we refer to as _dynamical constraints on learning_.

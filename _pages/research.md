---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

I am interested in the interaction of multiple learning pathways, both from an algorithmic perspective, as well as uncovering the multi-regional circuits that underlie learning. I am also interested in the neural dynamics that emerge over learning to support new task-relevant computations, with a focus on how feedback - sensory and internal feedback loops - can flexibly modulate effective cortical dynamics, and how these input-driven dynamics are learnt via multiple forms of errors.

### List of Projects:
1. [Feedback control of Cortical Dynamics](#1-feedback-control-of-cortical-dynamics)
2. [Data-driven models for control of biomechanical bodies](#2-data-driven-models-for-control-of-biomechanical-bodies)
3. [Population dynamics in the cerebellar cortex](#3-population-dynamics-in-the-cerebellar-cortex)
    - [Dynamics of electrically-coupled cerebellar inhibitory networks](#3a-dynamics-of-electrically-coupled-cerebellar-inhibitory-networks)
    - [Sensorimotor transformation across the cerebellar circuit](#3b-sensorimotor-transformation-across-the-cerebellar-circuit)
4. [Role of perceptual uncertainty in reward-driven learning](#4-role-of-perceptual-uncertainty-in-reward-driven-learning)
5. [Other projects](#5-ongoing-projects)
   - Learning without plasticity
   - Active learning for closed-loop experiments

## 1 Feedback control of Cortical Dynamics
---------------------------------------------------------
<img align="left" src="../../images/controlled.png" alt="Controlled dynamical system acting on downstream effector. Changes in the environment can be handled by feedback correction, changes in the control policy or changes to the dynamics." title="Learning in a controlled system." hspace=20px vspace=20px width="30%" />
I use _recurrent neural networks (RNNs)_ to model motor control tasks, including the use of motor BCI (brain-computer interfaces), where feedback about the output - either as _"efference copy"_ and/or _sensed state_ of the effector (limb, cursor, voice) - is a critical component to successful task completion. This feedback is needed to alter network dynamics in real time, in response to noise or external perturbations, to adjust the motor output. Moreover, learning in these networks may involve changes to the feedback inputs rather than to the recurrent network structure itself, especially when the dynamics are expressive enough. Borrowing insights from work on state-feedback controllers and modelling these "controllers" using neural network architectures, I study the implications of such an organization on __observed neural activity structure__ and __dynamical constraints on motor learning__.
<img align="left" src="../../images/constraint.png" alt="Dynamical constraints on learning. Controlled motor cortical activity can be adapted to use different BCI decoders, but the desired  trajectories are subject to dynamical, and not just geometric constraints. Image shows three sets of trajectories on a flowfield. One trajectory (T1) is along the flowfield and is easy, another trajectory (T2) is against the recurrent flowfield and requires large or infeasible inputs, and a third trajectory (T3) requires the neural state to firrst be pushed out in a less controllable direction in state space and is also difficult." title="Dynamical constraints on learning." hspace=20px vspace=20px width="80%" />

---------------------------------------------------------

## 2 Data-driven models for control of biomechanical bodies 
---------------------------------------------------------
<img align="left" src="../../images/biomech.png" alt="Neural network controller of biomechanical bodies simulated in physics engines, with realistic encoding of sensory feedback" title="" hspace=20px vspace=20px width="30%" />
Neuroscientists have long studied central pattern generators (CPGs) that generate oscillatory activity patterns for rhythmic motor outputs, such as for limbed locomotion. However, when a walking animal encounters an unexpected perturbation (e.g. uneven terrain, being pushed), it must integrate feedback from proprioceptive sensory neurons with ongoing rhythmic feedforward commands to adjust, recover, and sustain walking. I am using a data-driven integrative modeling approach to identify neural computations underlying robust locomotion in Drosophila (fruit fly model system) - modular neural network controllers, with biologically grounded models of proprioceptive sensing, controlling biomechanical models simulated with physics engines, and trained using imitation learning to produce realistic 3D kinematics. By manipulating the activity of proprioceptive neurons in silico and quantifying altered kinematics in these closed-loop models, I am able to identify the role of different classes of sensory feedback (joint positions, joint velocity, contact) in shaping walking behavior. In collaboration with John Tuthill at UW, I am also comparing these predictions to behavioral responses of actual walking flies to optogenetic activation of sensory neurons.

---------------------------------------------------------

## 3 Population dynamics in the cerebellar cortex
---------------------------------------------------------
The cerebellum - an important locus for motor learning and sensorimotor coordination - interacts reciprocally with the neocortex via disynaptic pathways. Cortico-pontine inputs enter the first stage of cerebellar processing as mossy fibre (MF) terminals, where expansion recoding at granule cells (GrCs) is suggested to transform these inputs into more learnable and separable representations. However, granule cell activity is critically regulated by a small but powerful inhibitory network of __Golgi cells (GoCs)__, which have been implicated in both homeostatic scaling and regulating GrC activity sparseness, dimensionality and spike timing.

During my PhD, I studied the __spatiotemporal structure of GoC network activity__, along with its relation to the feedforward mossy fibre inputs, to resolve how a small __electrically-coupled network__ may perform _such varied computational roles_.


### 3A Dynamics of electrically-coupled cerebellar inhibitory networks
---------------------------------------------------------
#### Two-photon imaging of Golgi cell network activity
<img align="middle" src="../../images/goc_imaging_all.png" alt=" Imaging of GCaMP6f-labelled cerebellar Golgi cells (GoCs)" title="Two-photon fluorescence microscopy in mice: Imaging of GCaMP6f-labelled cerebellar Golgi cells (GoCs)" hspace=20px vspace=15px width="100%" />
To examine the organisation of inhibitory population dynamics in the cerebellar granule cell layer, I used __3D random-access microscopy__ to monitor the activity of sparsely distributed Golgi cells. Using this approach, we desribed __multidimensional GoC population activity__, with both widespread and distributed components, that makes it well-suited for modulating the threshold and gain of downstream cerebellar granule cells and introducing spatiotemporal patterning. 

#### Dynamical regime changes with electrical connectivity topology
<img align="right" src="../../images/goc_sync.png" alt="dynamical regime changes with electrical coupling scale" title="Role of network coupling topology for synchronizability and stability of synchrony" hspace=100px vspace=15px width="80%" />
GoCs connect to each other via electrical synapses. We showed that network topology plays a role in determining the __stability of synchronous spiking__, as well as shaping slow dynamics. Moreover, experimentally-measured connectivity scale is close to a critical transition, resulting in __long input-driven transients but ultimately stable synchrony__. This allows us to posit new normative theories about the potential computational benefits of this dynamical regime. 



### 3B Sensorimotor transformation across the cerebellar circuit
---------------------------------------------------------
<img align="left" src="../../images/dual_imaging_A_B.png" alt="Fluorescence of MFs and GoCs and their respective activity eigenspectra" title="Simultaneous imaging of excitatory inputs (pontine mossy fibre inputs) and local inhibitory neurons (GoCs) within cerebellar cortex" width="99%" vspace=15px />
To further understand the role of structured inhibition in cerebellar computation, I used 3D random-access microscopy to monitor the activity of mossy fibre (MF) inputs simultaneously with GoCs in multiple paradigms - spontaneous behaviors, passive auditory stimuli, and throughout the acquisition of an auditory Go/No-Go task. By examining the plasticity of MF representations as well as how the relationship between inputs and GoC network activity changes during active behaviors, we test several theoretical predictions and provide a conceptual framework for the role of inhibition in shaping cerebellar cortical representations. Indeed, this adds to the growing consensus that even the primary stage of cerebellar processing shows task-specific adaptation and efficient representations, rather than a uniformly high-dimensional code.

---------------------------------------------------------

## 4 Role of perceptual uncertainty in reward-driven learning
---------------------------------------------------------

<img align="left" src="../../images/rewlearning.jpg" alt="Q-learning with perceptual uncertainty scaling" title="Behavioral and computational signatures of decisions guided by reward value and sensory confidence" hspace="90" vspace=15px width=800 />
_(Figure reproduced from [Lak et al, Neuron 2020](https://doi.org/10.1016/j.neuron.2019.11.018): Behavioral and computational signatures of decisions guided by reward value and sensory confidence)_

In a standard reinforcement-learning setting, expected returns are compared against true returns to modulate our learnt values and action policy. The "expected returns" or predictions are based on knowledge - or more accurately, our _inference_ - of our current state, and the actions we have recently taken ("Q-value tables"). However, uncertainty about our state should be reflected as uncertainty of reward prediction error, and thus the amount of learning at that time. This state uncertainty often stems from _perceptual uncertainty_ i.e. noisy or incomplete sensory information that we use for state inference. [Lak et al]((https://doi.org/10.1016/j.neuron.2019.11.018)) studied learning of a perceptual decision making task in mice, where mice had to choose appropriate motor actions based on noisy visual cues in order to get water rewards. We modelled the improvement in task performance as a reinforcement-learning process, where we modelled value as a combination of sensory confidence and reward. Fitting these models to the behavioural data offered a parsimonious explanation of the animals' sequence of choices and patterns of errors. 

---------------------------------------------------------

## 5 Ongoing Projects
---------------------------------------------------------

### Learning without Plasticity
Animals and humans show a remarkable ability to adaptively remap sensory flow into volitional movements, on timescales of seconds, minutes and hours. Much of this fast learning relies on activity-dependent processes - contextual and structure inference, input-driven reorganization of dynamics, and flexible association between brain areas. I am using network models and multi-region data to develop a theoretical and biological understanding of such learning without plasticity.

### Active learning for closed-loop experiments
Recent technological developments are increasing our ability to flexibly and dynamically manipulate large neural populations at a fine resolution. Such flexibility in the design of the spatiotemporal pattern of stimulation leads to a very high-dimensional control problem, which is not amenable to be solved by manual search. The challenge is further exacerbated by the complex neural connectivity and dynamics, which yield highly nonlinear and time-varying responses even to simple stimulation inputs, such as an impulse. In collaboration with Juncal Arbelaiz at Princeton University, I will use systems identification and optimization techniques for both "control for learning" and "learning to control" neural dynamics.





----------------------------------

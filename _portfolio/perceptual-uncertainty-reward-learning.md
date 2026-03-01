---
title: "Role of perceptual uncertainty in reward-driven learning"
permalink: /projects/perceptual-uncertainty-reward-learning/
excerpt: "Computational signatures of reinforcement learning when state inference is uncertain due to noisy perception."
tags:
  - reinforcement-learning
  - uncertainty
  - decision-making
  - data-driven
  - behavior
header:
  teaser: rl_small.jpg
---

<img align="left" src="../../images/rewlearning.jpg" alt="Q-learning with perceptual uncertainty scaling" title="Behavioral and computational signatures of decisions guided by reward value and sensory confidence" hspace="90" vspace=15px width=800 />
_(Figure reproduced from [Lak et al, Neuron 2020](https://doi.org/10.1016/j.neuron.2019.11.018): Behavioral and computational signatures of decisions guided by reward value and sensory confidence)_

In a standard reinforcement-learning setting, expected returns are compared against true returns to modulate our learnt values and action policy. The "expected returns" or predictions are based on knowledge - or more accurately, our _inference_ - of our current state, and the actions we have recently taken ("Q-value tables"). However, uncertainty about our state should be reflected as uncertainty of reward prediction error, and thus the amount of learning at that time. This state uncertainty often stems from _perceptual uncertainty_ i.e. noisy or incomplete sensory information that we use for state inference. [Lak et al]((https://doi.org/10.1016/j.neuron.2019.11.018)) studied learning of a perceptual decision making task in mice, where mice had to choose appropriate motor actions based on noisy visual cues in order to get water rewards. We modelled the improvement in task performance as a reinforcement-learning process, where we modelled value as a combination of sensory confidence and reward. Fitting these models to the behavioural data offered a parsimonious explanation of the animals' sequence of choices and patterns of errors. 
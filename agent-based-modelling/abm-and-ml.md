---
title: Using ABM and ML together
date: 2024-03-21
subject: Agent-based modelling
tags: [ABM]
bibliography: ../refs.bib
---

# Using ABM with Machine Learning
Using ABM and ML together can either be to improve the other method or complement each other. More details at [[improving-abm-ideas]] and [[making-predictions-with-abm]].

## Modelling non-physical systems 
Using agent-based modelling to model individual agents instead of complex systems. Model only the behaviour of the agents and how they interact with each other, which is easier than modelling entire systems. See Angione, C., Silverman, E., et al. (2022)[^angione2022using].

## Using ML to parameterise/calibrate agent-based models
 **Combine** supervised machine learning and intelligent sampling in the design of a *surrogate* meta-model, which constitutes a computationally cheap approximation of the real-model. The surrogate can then be deployed to explore the parameter space of the model at almost zero computation costs [^lamperti2018agent].

## Mapping inputs to outputs and performing sensitivity analysis
**ML** models that learn from the model outputs and approximate the best policies for different contexts??

  - not only the final output but at different time periods!!
  - identify the value of different parameters towards obtaining the desired outcomes?? - See Furtado, B. A. and Andreão, G. (2022) [^furtado2022machine]

Given the large number of variables we're likely to have in the model, ML (such as Bayesian Networks) can better represent the decision-making of agents in the real world, as opposed to improving the decision making itself.

  - help agents learn by enabling them to take into account their past experiences, and by observing what's happing to other agents
  - adapt their preferences in accordance with their experiences
  - cooperate with others to meet a mutual objective??

Also see Chen, S. H., Londoño-Larrea, P., et al. (2021) [^chen2021application]

## Segregation dynamics with reinforcement learning and agent based modelling
Reinforcement learning (RL) is a simulation method where agents become intelligent and create new, optimal behaviors based on a previously defined structure of rewards and the state of their environment. This method is referred to as Multi-Agent Reinforcement Learning (MARL) if multiple agents are employed. 

[^angione2022using]: [Angione, C., Silverman, E., et al. (2022), Using machine learning as a surrogate model for agent-based simulations.](https://doi.org/10.1371/JOURNAL.PONE.0263150)
[^lamperti2018agent]: [Lamperti, F., Roventini, A., et al. (2018), Agent-based model calibration using machine learning surrogates.](https://doi.org/10.1016/J.JEDC.2018.03.011)
[^furtado2022machine]: [Furtado, B. A. and Andreão, G. (2022), Machine Learning Simulates Agent-Based Model Towards Policy.](https://doi.org/10.48550/ARXIV.2203.02576)
[^chen2021application]: [Chen, S. H., Londoño-Larrea, P., et al. (2021), Application of Machine Learning Techniques to an Agent-Based Model of Pantoea.](https://doi.org/10.3389/FMICB.2021.726409/BIBTEX)

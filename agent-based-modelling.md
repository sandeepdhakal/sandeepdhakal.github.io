---
title: Agent-based modelling
date: 2023-02-01
subject: Agent-based modelling
tags: [ABM]
bibliography: refs.bib
---

# Introduction

Agent-based modelling is an approach to modelling complex and dynamic systems that are composed of _interactive, autonomous_ constituent entities (agents).

> A computer model that consists of a collection of agents that can take on a typically finite collection of states. The state of an agent at a given point in time is determined through a collection of rules that describe that agent's interaction with other agents or its environment. These rules may be deterministic or stochastic.
>
> - Laubenbacher, R., Hinkelmann, F., et al. (2013) [^laubenbacher2013agent]

Agent-based modelling and simulation (ABMS) is a powerful simulation technique that describes a complex, dynamic system. The structure of agent-based models is based on the interaction of heterogeneous, autonomous agents with each other and their environment. Agents may represent any number of unique entities of a particular type, for example individual people in the population of a city.

Often these models are spatially explicit, and the agents’ rationality is bounded (i.e., decision-making is not necessarily optimal and may depend on the context, as is often the case in reality). ABMS has been applied across most disciplines, including biology, social sciences, business, and archaeology; it is particularly suited for systems that are characterised by continual change and evolution through time and space.

ABMS is different from many other Artificial Intelligence techniques in terms of the higher priority placed on explanation than the predictions of the outcomes. Other tools and techniques might tell us more rapidly or accurately what might happen, but agent-based models help us understand the underlying reasons for why something might happen. Once validated, this can make ABMS extremely powerful to explore scenarios under novel system conditions that have no historic analogy (e.g., climate change).

One of the fundamental ideas of agent-based modelling is the idea of self-organisation. There is no central authority controlling how the agents behave. Rather, the agents interact with each other and their environment based on their goals and behaviours. _Self organisation_: individuals organise in a dynamic system without any central leadership.

The impacts of interactions between diverse individual agents humans, neighbourhoods, cities, or more abstract representations), or an individual agent with its environment (physical, social, information, etc.) can be felt at multiple scales as well as over differing timescales.

## A Simplified ABM

A typical agent-based model has three elements:

- a set of agents, their attributes and behaviours
- a set of agent relationships and methods of interaction
- the agents' physical, social, environmental context, etc.
  - Environments define the space in which agents operate, serving to support their interaction with the environment, and other agents. For example: social networks, grid cells, continuous space (GIS), etc.

## Properties of Agents

While the diversity of the application areas of ABM means we cannot have a consensus definition of an 'agent', there are several characteristics of agent that are common to most agents:

1. autonomous
2. heterogeneous
3. spatial
4. active:
5. some or all of:
   - goal-directed
   - reactive
   - bounded rationality
   - interactive/communicative
   - mobility
   - adaptation/learning

Rules are typically derived from published literature, expert knowledge, data analysis or numerical work and are the foundation of an agent's behaviour.

We can also incorporate behavioural frameworks within agent-based models to better represent human behaviour.

# When is ABM Suitable?

ABM is highly suitable for Systems that are characterised by continual change and evolution through time and space. In particular, the richness of detail one can take into account in ABMS makes it very appealing for the simulation of biological and social systems, where the behavior and the heterogeneity of the interacting components are not safely reducible to some stylized or simple mechanism.

---

## Applications of ABM

- Biological
  - cell behaviour and interaction, human immune systems, spread of epidemics
- Business & Technology
  - organisational behaviour, consumer behaviour, traffic congestion
- Socio-ecological Systems
  - decline of civilisations, collective behaviour of crowds, spread of invasive species in agricultural landscapes
- Epidemiology
  - COVID-19

## Bottom-up Generative Social Science

Agent-based models are generally more explanatory than predictive. They are characterised by self-organisation and emergent properties. These arise from the interactions of the agents and cannot be deduced simply by aggregating the properties of the agents.

Other methods might tell us what might happen, but agent-based models help us understand the reasons for why something might happen.

- What's the narrative?
- More amenable for policy-making

# Benefits of ABM

1. ABM captures emergent phenomena.
2. ABM provides a natural description of a system.
3. ABM is flexible.

# Challenges for ABM

1. Verification and validation of the models
2. Determining the right level of abstraction for the phenomena/system being studied.
3. Interpreting a model's outputs given that the output can be influenced by the model's initial conditions and rules of interaction, which are sometimes difficult to justify.
4. Efficiently and effectively simulating large-scale agent-based models, at the city-scale or the global scale.

---

# Examples of Agent-based models

## Understanding the Anasazi culture change through ABM

An attempt to recreate and explain the spatio-temporal history of the Anasazi people who occupied the prehistoric Long House Valley in northeastern Arizona, roughly between 1000 BC and 1300 AD [^dean2000understanding].

- Why did they abandon an area that could still support a substantial population?
- A physical and resource landscape, based on paleo-environmental and archaeological data available from different sources, forms the environment where the agents act.
- Agents represent individual households and agents have both individual and shared characteristics.

Results supported the assertion that socio-cultural 'pull' factors were responsible for their abandonment of the area.

# See Also

- [Using ABM and ML together](agent-based-modelling/abm-and-ml.md) for a discussion of how ABM and ML can be used together.

- [Improving agent-based models](agent-based-modelling/improving-abm-ideas.md) for how we can improve ABM using other technologies.

- [Making predictions with ABMS](agent-based-modelling/making-predictions-with-abm.md) for issues concerning making predictions using ABM.

[^laubenbacher2013agent]: [Laubenbacher, R., Hinkelmann, F., et al. (2013), Agent-Based Models and Optimal Control in Biology: A Discrete Approach.](https://doi.org/10.1016/B978-0-12-415780-4.00005-3)
[^dean2000understanding]: [Dean, J. S., Gumerman, G. J., et al. (2000), Understanding Anasazi Culture Change Through Agent-Based Modeling.](https://doi.org/10.1093/OSO/9780195131673.003.0013)

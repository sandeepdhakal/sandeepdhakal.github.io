---
bibliography: refs.bib
csl: chicago-fullnote-bibliography.csl
date: 2022-08-30
short-title: Digital Twins
suppress-bibliography: true
tags:
  - digital-twin
title: Digital Twins
---

# Introduction

The concept of a digital twin (DT) comes from industrial production and
space technology engineering and aims to optimise design and operations
of complex processes through a highly interconnected workflow[^1] [^2].
The origin of the Digital Twin is attributed to Michael Grieves and his
work with John Vickers of NASA. The initial description defines a DT as
a virtual representation of a physical product containing information
about said product, with its origins in the field of product life-cycle
management.

::: highlight-block
DTs are digital replicas of actual physical systems (living or not,
natural or manmade), interweaving solutions of complex systems analysis,
decision support and technology integration

Pylianidis, C., Osinga, S., et al. (2021)[^3]
:::

::: highlight-block
A dynamic virtual representation of a physical object or system, usually
across multiple stages of its life-cycle, that uses real-world data,
simulation, or machine learning models combined with data analysis to
enable understanding, learning, and reasoning. DT can be used to answer
what-if questions and should be able to present insights in an intuitive
way.

Verdouw, C., Tekinerdogan, B., et al. (2021)[^4]
:::

::: highlight-block
A virtual representation of a physical system (and its associated
environment and processes) that is updated through the exchange of
information between the physical and virtual systems.

VanDerHorn, E. and Mahadevan, S. (2021)[^5]
:::

## Essential characteristics of Digital Twins

After Verdouw, C., Tekinerdogan, B., et al. (2021)[^6]

- _timeliness_: (near) real-time updates such that changes in the
  physical object are (immediately) detected and synchronized with the
  digital twin.
- _fidelity_: unquestionable reliability
- _integration_: integrate data from different aspects of they
  physical world and ensure convergence in a consistent format.
- _intelligence_: include algorithms that describe, analyze or predict
  the behaviour of their physical twins.
- _complexity_: consider multiple interdependent objects as well as
  sub-systems at different levels of granularity.

## Why Digital Twins

DT have gained prominence, partially due to the uptake of Internet of
Things (IOT) technologies, that allow for the monitoring of physical
twins at high spatial resolutions, almost in real-time, through both
miniature devices and remote sensing, that produce ever-increasing data
streams.

The benefits of DT applications include reduced production times and
costs, hiding the complexity of integrating heterogeneous technologies,
creating safer working environments and establishing more
environmentally sustainable operations.

## Goals and objectives of DTs

- **decision making**: be the central hub for informed decision making
- **monitoring**
- **prediction**: help look into the future; produce reliable
  predictions and allow fully multivariate testing of scenarios
- **prescription**: suggest actions, interventions based on the
  current and future data and outcomes of scenarios and simulations
- **multi-dimensional**: integration of human, social, economic and
  other dimensions

# Attributes/Features

_convergence of monitoring and modelling_ :

- estimate uncertain model parameters and surrogate missing process
  details
- assimilate data from various external sources as well as the outputs
  of extensive simulations

_spatial_
: Spatially enabled DTs can provide valuable location-based insights,
helping users to understand place-based policy and planning issues,
test potential interventions, and deliver more sensible planning and
development [^7].

_virtual views_
: Multiple virtual views of the physical objects for different
stakeholders, decision-makers, scenarios, etc.

_nesting and integration_
: Allow the nesting or integration of DTs of different-scale, per
requirements. This can be more suited for virtual views based on
user requirements/privileges. For example, a DT of natural landscape
can be composed of DTs of farms, which can also be integrated more
readily with farm management systems, for example.

_agile_
: Make the best use of IT and AI, such as data-science, ML and ABM to
account for unknown processes and missing data and constraints. The
system should also be able to learn and adapt itself from previous
outputs and current and past measurements.

_interactive_
: Allow users to intervene, extract information and influence the
system trajectory across time and space[^8].

_transparent_ :

- When DTs are used to prescribe actions or make recommendations, it
  is important to make transparent the workings and underlying
  processes leading to them. In this aspect, the design of the UI is
  also important.
- At the same time, the risks associated with incomplete/incorrect DTs
  should be identified, along with any issues related to the
  recommendations

# Types of Digital Twins

Verdouw, C., Tekinerdogan, B., et al. (2021)[^9] have defined six types
of digital twins based on the goals and workings of the DTs. These are:

1.  Imaginary Digital Twin
2.  Monitoring Digital Twin
3.  Predictive Digital Twin
4.  Prescriptive Digital Twin
5.  Autonomous Digital Twin
6.  Recollection Digital Twin

![Types of Digital Twins](../images/verdouw-types-of-DTs.png)

# How are DTs different from models and simulations

A simulation refers to a digital model that imitates the operations or
processes within a system. Such simulations are used for analysing the
performance of systems and testing and implementing new ideas[^10].

A digital twin has to be associated with an object that actually exists:
a digital twin without a physical twin is a model. The concept of
similarity of two things throughout development and evolution is key to
the true digital twin, and for this similarity to be possible, the
physical twin must also exist.

- A simulation/model replicates what could happen, whereas a digital
  twin replicates what is happening
- If an object does not change much over time, or if data associated
  with that change cannot be captured, then a digital twin is not
  likely to be useful.

Although simulations and digital twins both utilize digital models to
replicate a system's various processes, a digital twin is actually a
virtual environment, which makes it considerably richer for study. The
difference between digital twin and simulation is largely a matter of
scale: While a simulation typically studies one particular process, a
digital twin can itself run any number of useful simulations in order to
study multiple processes.

Process understanding is core to science, and science can only progress
with deepening understanding of the associated processes and
interactions. There exist many process models (such as environmental
models) that offer sophisticated representations of underlying
phenomena/system/process. Process models are therefore core to digital
twins of the natural environment. However, process models do not, yet,
take advantage of the availability of large amounts of data; and they
can become more useful to digital twins only if they become more dynamic
structures that evolve over time.[^11]

## Why digital twins vs simulations/models?

The use of evolving data means that a key strength of the digital twin
approach is that it provides an accurate description of objects that
change over time. A validated model can provide a snapshot of the
behaviour of an object at a specific moment, but using that model within
a digital twin can extend the use of that model to timescales over which
the object and its behaviour will change significantly.[^12]

By having better and constantly updated data related to a wide range of
areas, combined with the added computing power that accompanies a
virtual environment, digital twins are able to study more issues from
far more vantage points than standard simulations can.[^13]

In addition to helping us extract new insights into extremes, change
points, thresholds, clusters, and correlations that can inform the
science (which can sometimes be done with data science or process
models), digital twins allow us to alter not just the state but
potentially the structure of the models or the mix of models in an
ensemble to gain meaningful insights that can inform our actions in the
opposite direction.[^14]

::: sticky-note
See [Digital Twins of natural or urban Landscape](digital-twins/dts-of-natural-and-urban-systems.md)
for discussion and some examples of digital twins of natural and urban systems.
:::

[^1]:
    Michael Grieves and John Vickers, "Digital Twin: Mitigating
    Unpredictable, Undesirable Emergent Behavior in Complex Systems,"
    _Transdisciplinary Perspectives on Complex Systems: New Findings and
    Approaches_, January 2016, 85--113,
    <https://doi.org/10.1007/978-3-319-38756-7_4>.

[^2]:
    David Jones et al., "Characterising the Digital Twin: A Systematic
    Literature Review," _CIRP Journal of Manufacturing Science and
    Technology_ 29 (May 2020): 36--52,
    <https://doi.org/10.1016/J.CIRPJ.2020.02.002>.

[^3]:
    Christos Pylianidis, Sjoukje Osinga, and Ioannis N. Athanasiadis,
    "Introducing Digital Twins to Agriculture," _Computers and
    Electronics in Agriculture_ 184 (May 2021): 105942,
    <https://doi.org/10.1016/J.COMPAG.2020.105942>.

[^4]:
    Cor Verdouw et al., "Digital Twins in Smart Farming,"
    _Agricultural Systems_ 189 (April 2021): 103046,
    <https://doi.org/10.1016/J.AGSY.2020.103046>.

[^5]:
    Eric VanDerHorn and Sankaran Mahadevan, "Digital Twin:
    Generalization, Characterization and Implementation," _Decision
    Support Systems_ 145 (June 2021): 113524,
    <https://doi.org/10.1016/J.DSS.2021.113524>.

[^6]: Verdouw et al., "Digital Twins in Smart Farming."
[^7]:
    [ANZLIC. _Principles for Spatially Enabled Digital Twins of the
    Built and Natural Environment in Australia_. (accessed 2021)](https://www.anzlic.gov.au/resources/principles-spatially-enabled-digital-twins-built-and-natural-environment-australia)

[^8]:
    Peter Bauer, Bjorn Stevens, and Wilco Hazeleger, "A Digital Twin
    of Earth for the Green Transition," _Nature Climate Change 2021
    11:2_ 11 (February 2021): 80--83,
    <https://doi.org/10.1038/s41558-021-00986-y>.

[^9]: Verdouw et al., "Digital Twins in Smart Farming."
[^10]:
    Louise Wright and Stuart Davidson, "How to Tell the Difference
    Between a Model and a Digital Twin," _Advanced Modeling and
    Simulation in Engineering Sciences_ 7 (December 2020): 1--13,
    <https://doi.org/10.1186/S40323-020-00147-4/FIGURES/4>.

[^11]:
    Gordon S. Blair, "Digital Twins of the Natural Environment,"
    _Patterns_ 2 (October 2021): 100359,
    <https://doi.org/10.1016/J.PATTER.2021.100359>.

[^12]:
    Wright and Davidson, "How to Tell the Difference Between a Model
    and a Digital Twin."

[^13]:
    IBM, "What Is a Digital Twin? \| IBM," 2022,
    <https://www.ibm.com/topics/what-is-a-digital-twin>.

[^14]: Blair, "Digital Twins of the Natural Environment."

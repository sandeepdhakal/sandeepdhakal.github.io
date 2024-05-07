---
title: Notes on Geographic Data Science
short-title: Geographic Data Science
date: 2023-04-15
subject: Geographic Data Science
tags: [GIS]
---

# Conceptual representations
- *Objects* are discrete entities that occupy a specific position in space and time.
- *Fields* are continuous surfaces that could, in theory, be measured at any location in space and time.
- *Networks* reflect a set of *connections* between objects or between positions in a field.

In the population density example, an "enumeration unit" is an object, as is a person. The field representation would conceptualize density as a smooth, continuous surface containing the total number of persons at all locations. The network representation would model the inter-related system of places whose densities arise from people moving around.

**Geographic tables** store information about discrete *objects*.

**Surface** data structures are used to record empirical measurements for *field* data models. For a field (in theory), there is an infinite set of locations for which a field may be measured. In practice, fields are measured at a finite set of locations. In practice, surfaces are recorded as uniform grids or arrays. For exmple, a surface for air pollution will be represented as an array where the rows and columns represent location (lat and lng).

**Spatial graphs** capture relationships between objects that are mediated through space; they are like geographic networks.


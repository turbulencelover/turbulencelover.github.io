---
layout: single
title: "Projects"
permalink: /Outreach/
header:
    overlay_image: /assets/images/bannerocean.jpeg
author_profile: true
classes: wide
---


# Undergraduate Projects

## 2022-2023

**Hidden skeleton of the ocean (4H project)**



The trajectories of fluid particles are sensitive to their initial positions,
which makes analysis based on single trajectories unreliable. For example, it is very hard to predict where a small dust goes once it is released in a fluid flow. Nevertheless,
there are patterns behind the trajectories that can be observed when some dye is released in the flow. These patterns, which can be interpreted as hidden skeletons of fluid flows, are identified as the most attracting or repelling surfaces (manifolds) in the flow. Some recent ideas that incorporate dynamical systems with fluid dynamics define robust material surfaces, namely **Lagrangian Coherent Structures (LCSs)**, shaping these patterns [1].

In this project, we investigate the fluid whose dynamics form the future of our planet and human race: **the ocean**. The LCS framework detects and even predicts key features of material transport in ocean currents. For instance, LCSs have been employed to predict the spread of oil in the Gulf of Mexico in 2010 [2]. In this project, after learning the mathematical foundation behind LCSs, the students will calculate them in ocean data to find where in these flows particles are attracted to or repelled from. Studying these structures can bring more insight to our understanding of climate and ocean dynamics. 

Most computational approaches to find LCS require seeding a large number of particles in flow and tracking them in time. This has drawbacks that include large memory demands, particle clustering and the complications of parallelisation and dealing with boundaries. In the second phase of this project, we try to borrow some ideas from the newly developed method of calculating Lagrangian means [3] to computing LCSs without tracking particles.

This project is well suited to students with strong programming skills, passion for fluid dynamics and interest in climate sciences.

[1] Peacock, Thomas, and George Haller. "Lagrangian coherent structures: The hidden skeleton of fluid flows." Physics today 66.2 (2013): 41.

[2] Olascoaga, María J., and George Haller. "Forecasting sudden changes in environmental pollution patterns" Proceedings of the National Academy of Sciences 109.13 (2012): 4738-4743.

[3] Kafiabad, Hossein A., and Jacques Vanneste. "Computing Lagrangian means." Journal of Fluid Mechanics 960 (2023): A36.


**Numerical simulation of stochastic differential equations (3H project)**

Stochastic differential equations (SDEs) are one of the fundamental tools for modelling financial, industrial, and scientific problems. In these equations, at least one of the terms is a stochastic process, resulting in a solution that is a stochastic process a well. To get a better feeling about SDEs and their difference with ordinary differential equation, consider the motion of a projectile in the air. If there is no wind (or the wind is a very well defined), we can find the exact trajectory of the projectile by solving a differential equation that comes from the laws of physics. If there is a randomly varying wind, we cannot determine the trajectory for every launch of the projectile. However, if we know the statistics of the wind (like its mean, variance and distribution), we can derive the statistics of the projectile trajectory, which is provided by the solution to a SDE. 

Although some basic concepts about stochastic processes and Brownian motion are reviewed in this project, our focus is developing **numerical methods** for solving SDEs. Hence, this project includes fair share of programming and is more suited to students who are interested in computational methods for solving mathematical problems that arise in various applications. The students are expected to be familiar with basic numerical methods for ordinary.

[1] Higham, Desmond J. "An algorithmic introduction to numerical simulation of stochastic differential equations." SIAM review 43.3 (2001): 525-546.

[2] Evans, Lawrence C. An introduction to stochastic differential equations. Vol. 82. American Mathematical Soc., 2012.
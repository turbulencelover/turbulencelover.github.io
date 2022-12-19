---
layout: single
title: "Research"
permalink: /Research/
header:
    overlay_image: /assets/images/NIW_anticyclone2.png
    caption: "*[Near-Inertial Wave Concentration inside Anticyclone](https://journals.ametsoc.org/view/journals/phoc/51/6/JPO-D-20-0257.1.xml).*"
author_profile: true
classes: wide

---
## Computing Lagrangian Means Without Particle Tracking

<div style="width:95%;  padding-center: 10px; float:top">
    {% include figure image_path="/assets/images/Vorticities_new.png" caption ="*Vorticity field and its Lagrangian and Eulerian means in a shallow-water simulation: (a) instantaneous vorticity, (b) Lagrangian mean vorticity, and (c) Eulerian mean vorticity. Panels (b) and (c) share the same colourbar shown to the right of panel (c). More details in [Kafiabad & Vanneste 2022](https://arxiv.org/pdf/2208.02682.pdf).*"%}
</div>

<div style="font-size:19px; text-align: justify"> 
Time averaging is an essential tool in analysing multi-timescale flows and can be performed in two ways: 1) <b>Eulerian</b> and 2) <b>Lagrangian</b>. The Eulerian mean is the average of flow variables at fixed spatial points, whereas the Lagrangian mean is the average of flow variables along particle trajectories. Lagrangian averaging has several pivotal advantages over its Eulerian counterpart. One of these advantages is demonstrated in the figure above, where a high-amplitude wave is interacting with turbulent shallow water. The strong wave – present in the instantaneous vorticity field (panel (a)) – is filtered out after both types of averaging. However, Lagrangian averaging (panel (b)) has preserved the small-scale features of the flow that are blurred by Eulerian averaging (panel (c)). Lagrangian averaging also removes the Doppler shift that eclipses the separation of time scales between the background flow and waves leading to a more reliable decomposition of the two. Despite its advantages, the widespread adoption of Lagrangian averaging has been hindered by computational complications. To compute the Lagrangian mean in numerical models usually particles are tracked using interpolated velocities at particle positions at every time steps, which requires substantial memory usage and is ill suited for efficient computational parallelisation. <br>

We propose a novel numerical method to compute Lagrangian means that does not require tracking particles and consquently circumvents these difficulties. In this approach, we compute the Lagrangian mean as solutions to a set of Partial Differential Equations (PDEs) integrated over the averaging interval. This paradigm could be a breakthrough in computing Lagrangian means as these PDEs can be discretised in a variety of ways and solved on-the-fly (i.e. simultaneously with the dynamical governing equations). Hence, they do not require storing any time series and substantially reduce the memory footprint compared to particle tracking.
</div>

<span style="font-size:19px;"> For more details see the following papers: <br> </span>
<span style="font-size:18px;"> 1. [Kafiabad. "Grid-based calculation of the lagrangian mean." *Journal of Fluid Mechanics*, 940, 2022.](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/E4E2A6F496D7CCEFC6BFC7353E478E9E/S0022112022002336a_hi.pdf/grid-based-calculation-of-the-lagrangian-mean.pdf) <br> 2. [Kafiabad and Vanneste. "Computing Lagrangian Mans." *Under revision for Journal of Fluid Mechanics*, 2022.](https://arxiv.org/pdf/2208.02682.pdf) </span>

<span style="font-size:19px;"> Early version of this work is presented in [this talk](https://www.youtube.com/watch?v=PAo5Ahv4JCY) for the University of Hamburg. </span>
 
## Scattering of Inertia-Gravity Waves by Geostrophic Turbulence


<center>
<video width="80%" height="auto" max-height="90%" controls="controls">
  <source src="/assets/images/Scattering_totvort-wavew_lr.mp4" type="video/mp4">
</video>
</center>
<p style="font-family:caption-font-family; font-size:type-size-2; margin-bottom: 0.5em; text-align:justify"><i>Two horizontal slices of 3D Boussinesq simulation initiated by geostrophic turbulence superimposed with a monochromatic plane wave. Left: total vertical vorticity, right: wave's vertical velocity. </i>
</p>

<div style="font-size:19px; text-align: justify"> 
Inertia-gravity waves generated from different sources such as tides, topography and convection scatter as they travel through the large-scale atmospheric and oceanic vortices. This scattering process is shown in the above video where a monochromatic plane wave is superimposed with geostrophic turbulence in a 3D Boussinesq simulation. As it can be seen, the wave field (shown in the right panel) eventually loses its preferred direction and develops small scale features. The interaction of these waves with the slowly moving vortices has very important implications in the energetics and the dynamics of geophysical flows. Relying on the statistical isotropy and stationarity of vortices and their temporal (and spatial) scale separation with waves, we have put forward a theory that describes the evolution of wave energy in Fourier space. More specifically, it predicts that the waves energy diffuses on constant frequency surfaces, which are double cones in 3D Boussinesq flows (see the figure below). When the forced waves reach a steady state, this theory shows that the wave energy spectrum scales as <math>k<sup>-2</sup></math> (k being the wavenumber). This provides a possible answer to the long-standing question of the mechanism underpinning the observed atmospheric spectra.<br>
</div>
<span style="font-size:19px;"> For more details see the following papers: <br> </span>
<span style="font-size:18px;"> 1. [Kafiabad, Savva, and Vanneste. "Diffusion of inertia-gravity waves by geostrophic turbulence." *Journal of Fluid Mechanics*, 869:R7, 2019.](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/31E102FB36D4066476A6A5862B4BFCD8/S0022112019003008a.pdf/div-class-title-diffusion-of-inertia-gravity-waves-by-geostrophic-turbulence-div.pdf) <br> 2. [Cox, Kafiabad, and Vanneste. "Inertia-gravity-wave diffusion by geostrophic turbulence: the impact of flow time dependence." *Under revision for the Journal of Fluid Mechanics*, 2022.](https://arxiv.org/pdf/2207.09386.pdf) <br> 3. [Savva, Kafiabad, and Vanneste. "Inertia-gravity-wave scattering by three-dimensional geostrophic turbulence." *Journal of Fluid Mechanics*, 916:A6, 2021.](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/824E2E5BDAC7C940D25F49923315DB78/S0022112021002056a.pdf/inertia-gravity-wave-scattering-by-three-dimensional-geostrophic-turbulence.pdf)</span>

Considering it a breakthrough, the Journal of Fluid Mechanics selected our work for the Focus on Fluid article, where an invited expert wrote the following review about our findings:

<span style="font-size:19px;">[Young. "Inertia-gravity waves and geostrophic turbulence." *Journal of Fluid Mechanics*, 920, 2021.](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/DF08A67338F0506C35DE2C8FD557813E/S0022112021003347a_hi.pdf/inertia-gravity-waves-and-geostrophic-turbulence.pdf)</span>

<div style="width:95%;  padding-center: 10px; float:bottom">
    {% include figure image_path="/assets/images/Cone_WaveVel.png" caption = "*Scattering of a plane inertia-gravity wave by a turbulent geostrophic flow. Top row is the vertical velocity field for z = 0,
and bottom row is the representation of the wave energy distribution in Fourier space at four successive times (increasing from the left to right). The constant-frequency cone associated with the frequency of initial plane wave is shown by the stripes; small-, medium- and large-sized dots indicate wave energy density exceeding, respectively, 0.004%, 0.02% and 0.2% of the initial wave energy.*"%}
</div>




## Efficient Computation of Wave Transport and Scattering

<div style="font-size:19px; text-align: justify"> 
Atmospheric and oceanic (internal and surface) waves typically have wavelengths that are smaller than the grid size of operational numerical models; as a result, they cannot be fully resolved. Fortunately, the phase of these waves is irrelevant to their impact, and it is sufficient to model their phase-averaged properties that are felt at the grid size of numerical models. This process of phase-averaging, however, leads to a set of new equations that depend on three-dimensional wavenumbers in addition to three-dimensional spatial coordinates. The high-dimensionality of these equations poses a new computational challenge. In this project, we address this challenge by applying the mathematical technique termed dynamical low-rank approximation to reduce the e ective dimensionality of the problem. This approach has a
great competitive edge over the alternatives, because it judiciously reduces the computations and can be parallelised very efficiently . This is a work in progress.
</div>

## Interaction of Near-Inertial Waves with Vortices

<center>
<video width="90%" height="auto" controls="controls">
  <source src="/assets/images/wavekineng_totvort.mp4" type="video/mp4">
</video>
</center>
<p style="font-family:caption-font-family; font-size:type-size-2; margin-bottom: 0.5em; text-align:justify"><i>Horizontal slices of a 3D Boussinesq simulation initialised by a strong inertial wave and an anticyclone. Left: the wave kinetic energy. Right: total vertical vorticity. </i>
</p>

<div style="font-size:19px; text-align: justify"> 
Near-inertial waves (NIWs) are generated at the ocean surface and are one of the main reservoirs of kinetic energy in the ocean. Hence, their interaction with the eddies and vortices are very important. Anticyclonic vortices focus and trap these waves so that near-inertial energy levels are elevated within the vortex core. This is demonstrated in the video above, which is a simulation of a high-amplitude inertial wave interacting with an anticyclone. The left panel shows the wave energy in a horizontal slice of this flow and the right shows the vertical vorticity at the same slice which is affected by waves oscillations. The waves kinetic energy is periodically trapped in this vortex in a time scale much slower than the inertial period (i.e. the wave period). We investigate some aspects of this process, including the nonlinear modification of the vortex by the wave and the frequency of wave trapping, using analytical tools which are compared against the high-resolution simulation of the Boussinesq equations. 
</div>

<span style="font-size:19px;"> For more details see the following papers: <br> </span>
<span style="font-size:18px;"> 1. [Kafiabad, Vanneste and Young. "Interaction of near-inertial waves with an anticyclonic vortex." *Journal of Physical Oceanography*, 05 Apr. 2021.](https://journals.ametsoc.org/view/journals/phoc/51/6/JPO-D-20-0257.1.xml) <br> 2. [Kafiabad, Vanneste and Young. "Wave-averaged balance: a simple example." *Journal of Fluid Mechanics*, 911:R1, 2021.](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/A8FFD5F4256E74684701EB70235A5ED2/S0022112020010320a_hi.pdf/wave-averaged-balance-a-simple-example.pdf) <br>
</span>

## Breakdown of Balance Dynamics from a Turbulence Perspective

<center>
<video width="90%" height="auto" controls="controls">
  <source src="/assets/images/balance_breakdown_lr.mp4" type="video/mp4">
</video>
</center>
<p style="font-family:caption-font-family; font-size:type-size-2; margin-bottom: 0.5em; text-align:justify"><i>Vertical vorticity at a horizontal and a vertical slice of 3D Boussinesq simulation.Only a part of domain is shown. </i>
</p>

<div style="font-size:19px; text-align: justify"> 
Balance models (such as geostrophic balance) reduce the full equations to a simpler set to describe large-scale atmospheric and oceanic flow. Their solutions, however, can spontaneously generate imbalance in the context of the full equations. To study this phenomenon, we perform high-resolution turbulence simulations of the non-hydrostatic Boussinesq equations, starting with a high-order nonlinearly balanced
initial condition (which is the next-order improvement to quasigeostrophic). The above videos is an example of Boussinesq simulation (only a part of domain shown), which shows that imbalance is generated in time in some regions of this flow. By increasing the dimensionless parameters such as Rossby and Froude, we then investigate at what scales balance breaks down and after how long. 

Our results show that the balanced initial condition displays a steep geostrophic energy spectrum and an even steeper ageostrophic energy spectrum. However, a shallow tail later develops in the ageostrophic energy spectrum at small scales if Ro and the Reynolds number, Re, are large enough. This shallow range moves toward smaller wavenumbers if Ro is increased.
</div>

<span style="font-size:19px;"> For more details see the following papers: <br> </span>
<span style="font-size:18px;"> 1. [Kafiabad and Bartello. "Spontaneous imbalance in the non-hydrostatic boussinesq equations." *Journal of Fluid Mechanics*, 847:614-643, 2018.](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/balance-dynamics-in-rotating-stratified-turbulence/02EB47344C3CA3D890990A74CD03E93F) <br> 2. [Kafiabad and Bartello. "Rotating stratified turbulence and the slow manifold." *Computers & Fluids*, 151:23-34, 2017.](https://www.sciencedirect.com/science/article/abs/pii/S0045793016303218) <br> 3. [Kafiabad and Bartello. "Balance dynamics in rotating stratified turbulence. *Journal of Fluid Mechanics*, 795:914-949, 2016.](https://scholar.google.co.uk/citations?view_op=view_citation&hl=en&user=Rv1ZtYAAAAAJ&citation_for_view=Rv1ZtYAAAAAJ:_FxGoFyzp5QC) <br>
</span>

<span style="font-size:19px;"> A part of this project is presented in [this talk](http://www.birs.ca/events/2018/5-day-workshops/18w5119/videos/watch/201802221431-Kafiabad.html) for the Banff International Research Station. </span>



## Lagrangian Coherent Structure for Detection of Airflow Distrubances over Airports

<div style="width:49%; padding-left: 10px; float:left">
    {% include figure image_path="/assets/images/HKIA_map.jpg" caption = "*Topography of Hong Kong International Airport and its surroundings.*"%}
</div>

<div style="width:50%; padding-right: 10px; float:right">
    {% include figure image_path="/assets/images/Lidars.jpg" caption = "*Geometry of scans by the lidar, with elevation angles of 1.4° (green) and 3° (blue). Dimensions are in meters.*"%}
</div>


<div style="font-size:19px; text-align: justify"> 
The short-term prediction of disturbances encountered by aircraft in the last minutes of landing provides safer and more comfortable flight for passengers. In this project, we aim to evaluate the use of Lagragian Coherent Structures (LCSs) for detecting these disturbances over the Hong Kong International Airport. This airport is a great case study as topography-induced wind shear and air-sea interactions create a substantial amount of aerial turbulence (see the geographical location of the airport in the figure). We compute LCSs using the 2D velocity field retrieved from Lidar scans (shown in the figure) for the detection of disturbances and compare them against historical landing data and pilot reports.
</div>

<span style="font-size:19px;"> For more details see: <br> </span>
<span style="font-size:18px;"> [Kafiabad , Chan, and Haller. "Lagrangian detection of wind shear for landing aircraft." *Journal of Atmospheric and Oceanic Technology*, 30(12):2808-2819, 2013.](https://journals.ametsoc.org/view/journals/atot/30/12/jtech-d-12-00186_1.xml)
</span>



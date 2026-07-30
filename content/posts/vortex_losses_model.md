+++
date = '2025-09-24T16:12:25-10:00'
draft = false
title = 'Modeling vortex shedding in linear solvers'
tags = ["linear theory", "energy dissipation", "modeling", "OWC"]
+++

![vortex](/images/vortex/lin2025_fig5.png)\
<small>Vorticity at the front chamber edge of an OWC (Taken from Figure 5 of [Lin et. al., (2025)](https://pubs.aip.org/aip/pof/article-abstract/37/6/065173/3350964/Experimental-investigation-of-vortex-induced-flow?redirectedFrom=fulltext)).</small>

Modeling ocean structures like wave energy converters and coastal structures typically use models based on potential flow theory to provide guided decision making for the design of such structures and devices. This is due to the fast computational time of such models.  
However, such models typically neglect viscous damping of energy e.g. energy dissipation due to vortex shedding and hence for wave energy devices results to overprediction in estimated power efficiency obtained from the linear model. 

For Oscillating water column (OWC) wave energy converters, viscous dissipation is typically dominant at the chamber edges. 
In this study, we would like to consider such dissipation in the potential flow framework. 
Previous work have focused on either empirically correcting to include viscous dissipation or artificially include the dissipation as viscous damping on the free surface boundary condition.
Both provide a simple fix, however do not give us coefficients that would have physical meaning. 

In this work, we propose attaching a perforated region at submerged chamber edges of the OWC, to account for vortex-induced viscous losses. 
We first perform this for two plates separated by a given distance. 
Attaching a perforated region would allow for the dissipation of energy using two main parameters (1) the perforated region size, and (2) the damping coefficient. 
Our recent [paper](https://www.mdpi.com/2073-4441/18/5/608) successfully models this and shows that a constant dissipation parameter can be obtained from a wide range of perforated region sizes.

![vortex2](/images/vortex/reyes2026_fig1.png)\
<small>Modeling energy dissipation with a short perforated region attached to the plate edges (Taken from Figure 1 of [Reyes and Huang, (2026)](https://www.mdpi.com/2073-4441/18/5/608)).</small>

We are currently extending the theory to consider the OWC, and will come up shortly in a follow up paper. Stay tuned!

<!-- By using this model, engineers are able to consider energy losses due to vortex shedding in the design optimization stage, which will save time and money in the final design stages, where time consuming CFD simulations are performed.  -->

<!-- complete modeling framework in order to account for vortex induced losses in linear solvers. 
We perform the approach for a simple case of a single submerged vertical plate and extend this for the case of two vertical plates. 
This is performed by introducing a porous region at the submerged ends of the vertical plates. 
We determine the spatial extent of the porous region by performing a sensitivity of the reflection coefficient, while the dissipation coefficient is obtained by an optimization with a existing loss curve.
This methodology is easy to apply to multiple plates and can be easily performed on various geometries provided the availability experimental test results. 
By using this model, engineers are able to consider energy losses due to vortex shedding in the design optimization stage, which will save time and money in the final design stages, where time consuming CFD simulations are performed.  -->

<!-- I am working on a short manuscript to demonstrate this methodology, hopefully it will be released soon!  -->

<!-- In this study we develop an analytical model in order to optimize and further understand the physical mechanisms behind the proposed [hybrid breakwater](https://clintreyes2.github.io/clintreyes.github.io/posts/owc_expt/) design which incorporates a wave energy converter into a slotted breakwater.
The theory is governed by linear potential flow with a non-linear pressure drop boundary condition at the internal air-water interface of the oscillating water column (OWC) air chamber. The slotted breakwater is also modeled with a pressure drop boundary condition, however a linear implementation is used as existing studies (Suh et al., 2006) show sufficient applicability of the linear model. A dimensional analysis was performed to determine important parameters. 

Sketch of the theoretical model: 
![sketch_theory](/images/owc_theory_sketch.png)

Results show that the chamber width is the main controlling parameter for changing the peak and range of operational frequencies at which the OWC operates. 
Decreasing the size of the slots or the slotted breakwater porosity provides increase in energy extraction efficiency and decrease in wave transmission. However, an increase in wave reflection and total horizontal force on the structure must be accounted for. 
It was shown that under increasing amplitudes, the energy extraction efficiency also increases while dropping the relative wave transmission through the breakwater. Finally the variations is chamber draft at the scale of tidal changes show minimal effects for long waves, however might be important for shorter or deep water waves. 

This work was presented in the 41st International Association for Hydro-environment Engineering and Research (IAHR) world congress held on June 21-27, 2025 in Singapore. 
Upon discussions with a colleague at the conference, the importance of the energy dissipation at the chamber tips may have quite a significant impact when looking into the effect of the wave amplitude. 
Work is currently ongoing on developing a model to include this phenomenon in existing linear models.  -->


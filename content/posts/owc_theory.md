+++
date = '2026-07-29T16:12:25-10:00'
draft = false
title = 'Analytical modeling of a wave energy extracting breakwater'
tags = ["potential flow", "modeling","wave energy", "OWC", "breakwater", "non-linear PTO"]
+++

![figure](/images/analytical/r1_OWCbreakwater_illust_3c.jpg)
<small>Figure 1 from [Reyes and Huang (2026)](https://www.sciencedirect.com/science/article/abs/pii/S0029801826030568).</small>

In this study we developed an analytical model of a [hybrid breakwater](https://clintreyes2.github.io/clintreyes.github.io/posts/owc_expt/) design which incorporates a wave energy converter with a slotted breakwater.
The theory is governed by linear potential flow with a non-linear power take-off or PTO. This allows for modeling a non-linear turbine such as impulse turbines as well as orifices which are typically used in laboratory tests. 
The slotted breakwater is parameterized as in Suh et al., 2006. 

Sketch of the theoretical model: 
![sketch_theory](/images/analytical/owcsb_sketch3.png)
<small>Figure 2 from [Reyes and Huang (2026)](https://www.sciencedirect.com/science/article/abs/pii/S0029801826030568).</small>

Results show that the chamber width is the main controlling parameter for changing the peak and range of operational frequencies at which the OWC operates. 
Decreasing the size of the slots or the slotted breakwater porosity provides increase in energy extraction efficiency and decrease in wave transmission. However, an increase in wave reflection and total horizontal force on the structure must be accounted for. 
Modeling with a nonlinear PTO allows us to observe the effects of increasing wave amplitude, which generally cannot be observed from linearized PTOs. 
Results show that under increasing incident wave heights, the pneumatic extraction efficiency also increases while dropping the relative wave transmission through the breakwater. 
Finally the variations is chamber draft at the scale of tidal changes show minimal effects and can be ignored. 

This work was presented in the 41st International Association for Hydro-environment Engineering and Research (IAHR) world congress held on June 21-27, 2025 in Singapore. 
Upon discussions with a colleague at the conference, the importance of the energy dissipation at the chamber tips may have quite a significant impact when looking into the effect of the wave amplitude. 
We are currently working on developing a [model](https://clintreyes2.github.io/clintreyes.github.io/posts/vortex_losses_model/) to include this phenomenon in present linear potential flow based models. 

Update: [This work](https://www.sciencedirect.com/science/article/abs/pii/S0029801826030568) has been published in Ocean Engineering! \
Preprint : [PDF](/pdf/OE_RH26_preprint.pdf) \
Supplementary material on the numerical implementation can be found here: [![DOI](https://zenodo.org/badge/1317025962.svg)](https://doi.org/10.5281/zenodo.21700609).

If you would like to use the code to obtain the wavenumbers (real and imaginary) from the dispersion relation, you can find it here: [![DOI](https://zenodo.org/badge/1318935136.svg)](https://doi.org/10.5281/zenodo.21732032)

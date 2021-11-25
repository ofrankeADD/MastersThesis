# Master's Thesis

## Title

Simulating AGN-inflated bubbles with anisotropic viscosity on a moving mesh

## Abstract

Feedback of the active galactic nucleus (AGN) to the ambient intracluster medium (ICM) leads to complex structures in the center of a galaxy cluster and is of crucial importance for solving the cooling-flow problem.
Dynamics of AGN-inflated underdense bubbles provide an important source of heating as they buoyantly rise through the cluster atmosphere. The evolutionary effects and heating of the ICM thereby critically depend on the bubble morphology.

Ideal inviscid hydrodynamical simulations cannot reproduce the observed coherent morphology, because the artificial bubbles become unstable to Rayleigh-Taylor instability (RTI) and Kelvin-Helmholtz instability (KHI) and dissolve into the ICM on much shorter time-scales than their observed lifetimes.
Therefore, additional physics have been considered to be important to preserve the bubble stability, including magnetic fields and viscosity.
Since the ICM is a weakly collisional, magnetized plasma, where the collision mean free path of the ions is much larger than their Larmor radius, microscopic transport of momentum and heat becomes highly anisotropic. 

Hence, we perform Braginskii-magnetohydrodynamic simulations in an isothermal cluster core employing the moving-mesh code _AREPO_ while applying adaptive mesh refinement. For the first time, we quantify parallel viscous heating rates of buoyantly rising bubbles to clarify whether viscous heating can offset radiative cooling and study the significance of Braginskii viscosity on the bubble dynamics.

We show that Braginskii viscosity mainly suppresses RTI and KHI parallel to the magnetic field lines, while having minor effects on modes perpendicular to the field.
We find that anisotropic viscous dissipation of turbulent motions is not very efficient in heating the ICM in a volume filling fashion.
Since the viscous heating rate is sensitive to pressure anisotropy, it can be suppressed if microscopic plasma instabilities are triggered, which pin the pressure anisotropy down to certain limits for marginal stability. 

Simulating cluster atmospheres with magnetic fields having &beta;=100 reveals an invariance in bubble evolution in terms of mixing efficiency and viscous heating rates regardless of whether pressure anisotropy is limited or not. If so, micro-scale instabilities are rarely triggered effectively resulting in unsuppressed Braginskii viscosity.

If however the magnetic tensions are negligibly weak (&beta;=10^6) the bubble evolution is drastically altered depending on whether the pressure anisotropy is bounded within levels of marginal stability. If so, viscous stresses are highly suppressed by the microinstabilities such that they can no longer prevent the bubbles from disruption, resembling the inviscid case.

## Results

![reyn3D_higher_mhd_x_b1e6_brag_d1e-2_3_lim_iso_cyc_clumping_S91_bub1e-20](https://user-images.githubusercontent.com/49908052/143506264-fb489280-eab0-4259-a03e-16037e20baeb.png)
Volume-integrated dye entropy _S_ as a function of time, normalised by the maximum entropy S<sub>max</sub> for a fully mixed dye concentration. A fully mixed cluster has S/S<sub>max</sub>=1. It shows the mixing efficiency of the bubble material for the given runs or in other words how viscous the evolving bubbles become.

--------------------------------------------------------------------------------------------------

![reyn3D_higher_mhd_x_b1e6_brag_d1e-2_3_lim_compare_pass_log_res1024_proj_bub0001](https://user-images.githubusercontent.com/49908052/143506308-e5d7fa8c-3a9b-44a1-9505-ba2ff23a4396.png)
Projected slices of the x-y midplane parallel to the initially uniform magnetic field lines showing the tracer mass fraction X<sub>bub</sub> for several models including from left to right _hydro_, _xB6N2lim_, _xB6N3_ and the fiducial run _xB6N2_. Each panel spans a spatial domain corresponding to dimensions x in [-1.5r<sub>0</sub>, 1.5r<sub>0</sub>] and y in [0, 3r<sub>0</sub>]. The thin projections in z-direction have width dr=0.066r<sub>0</sub> centered at z=0.

--------------------------------------------------------------------------------------------------

![reyn3D_higher_mhd_t_b1e2_brag_d1e-2_lim_compare2_tB2N2lim_res1024_proj](https://user-images.githubusercontent.com/49908052/143505935-a79e6a2a-29e1-4a8e-b108-5a0d47bc4ffa.png)
Projected slices of the x-y midplane showing from left to right the magnetic field strength in micro Gauss, the plasma beta, the absolute vorticity, the limited pressure anisotropy, the departure from marginal stability _fp_ and the viscous heating rate. The first and second columns show streamlines of the magnetic vector field, while the third column shows the vector field of the velocity. Each panel spans a spatial domain corresponding to dimensions x in [-1.5r<sub>0</sub>, 1.5r<sub>0</sub>] and y in [0, 3r<sub>0</sub>]. The thin projections (except for _fp_) in z-direction have width dr=0.066r<sub>0</sub> centered at z=0.



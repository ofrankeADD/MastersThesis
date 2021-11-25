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

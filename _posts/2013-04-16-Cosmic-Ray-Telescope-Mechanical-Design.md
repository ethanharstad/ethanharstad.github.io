---
layout: post
category: Electronics
tags: [Cosmic Ray Detector]
---
As discussed in a previous post, I am in the process of developing a cosmic ray telescope for use by several universities on stratospheric balloons. The major components of the system include two plastic scintillator panels, an electronics package (power supply, amplifier, conditioner and coincidence counter), inertial measurement unit, data logger and the mechanical assembly to hold all the parts together. This post will discuss the design of the mechanical assembly.

The factors contributing to this design are:

-   Easily reproduceable
   
    Many schools and groups may want to reproduce this design. Expensive and complex equipment should be avoided as much as possible.

-   Easily reconfigurable
    
    A major factor in coincidence count rates is the solid angle exposed by the two detector plates which is a function of the distance between them. This distance should be able to be changed with minimal effort.
    
-   Durable
    
    Stratospheric balloon payloads are exposed to near vacuum and temperatures as low as -60C as well as high vibrations and of course the impact of landing. Any experiment needs to be design and built to withstand these effects, especially an experiment of this expense.
    
-   Non-magnetic

    The cosmic particles of interest are able to pass through several inches of lead so metal is acceptable and sometimes even desired (controlling or even exploiting compton scattering). However, the particle flux is dependent on the magnetic field which will be measured by this experiment, therefore we must make an effort not to distrub those measurement.

Several design concepts were proposed, ranging from the fairly standard balloon payload of foam and duct tape to laser cut assemblies and even 3D printed components. One concept that kept coming up was extruded aluminum profiles. Profiles are available in pre-cut lengths and some distributors will even drill holes for you. The t-slots in the profiles and wide range of fasteners would make the system highly reconfigurable. These factors lead us to chose standard 1" 80/20 aluminum profiles as the main component of the structure. One of the smaller options (MicroRax, Maker Beam, Open Beam, etc) would have been lighter but do not have a slot large enough to accomodate the thickness of scintillator we had planned (requiring an expensive milling machine to modify the profile).

After deciding on our profiles, we proceeded to develop the actual assembly. We needed to constrain the scintillator panels, hold them parallel and allow the distance between them to be changed. These requirements naturally lead to a concept of framing the panels and installing the frames on long rails to hold them parallel and allow the distance to be set.

Because the 1" aluminum extrusions weigh about half a pound per foot, minimizing the overal length of the profiles used is critical. We used a kinematic constraint approach to identifying redundant stucture. The final design eliminated one of the long sliding rails and traded three sided scintillator frames for one lateral profile, instead using the sliding rails to constrain the scintillators. The final design is pictured below, as well as a link to the SketchUp file.

![Mechanical Overview](/assets/images/CosmicRayTelescope/MechanicalOverview.png)
[SketchUp File](https://github.com/ethanharstad/SiPMCosmicRay/blob/master/Mechanical/TelescopeAssembly.skp)
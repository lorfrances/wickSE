# wickSE
These 3 files were developed for use in the Surface Evolver (SE) (https://kenbrakke.com/evolver/evolver.html) for 3-D numerical simulations of the capillary surface and pressure in evaporating wick structures. Results from these simulations have been published:
> L. Franceschetti, Y. Kameya, M. Kaviany, "3D-printed, ceramic porous metasurface wick: hexagonal-prism unit-cell capillary evaporator," _Int. J. of Heat and Mass Transfer_, **246, 127041,** 2025.

If you use these codes in your work, please cite the above publication.

The files include:

  (1) A 3D-printed wick microstructure (unit-cell) with the meniscus facing outward on the open plane (1/6 geometry by symmetry).
  
  (2) Spherical particle (unit-cell) for use in a hexagonal packing arrangement. It is also sintered to the substrate (1/8 of the diameter is truncated in vertical direction).
  
  (3) The same 3D-printed wick microstructure of (1), including a central strut (1/6 geometry by symmetry).
  
Images of sample results are shown below.

<img src="https://github.com/lorfrances/wickSE/blob/main/sample_meni.png" width="400">

<img src="https://github.com/lorfrances/wickSE/blob/main/sample_mono.png" width="400">

## Usage
The use of the files is straightforward following installation of SE. To change the dimensionless capillary pressure to observe the corresponding change in the capillary surface, modify the line specifying (enclosing) the body and its volume:
> bodies:
> pressure -x.xxxx

A few useful functions are provided. These can be run as commands in SE:
> stl: Writes an STL file containing faces and vertices

> Run_ALL: Preforms some refinement and calculation steps to iterate toward the minimized free surface. This may or may not be close to the converged result (although it has worked for me).

> liq_thik3: Used to write to file the thickness (elevation) of all vertices on the liquid surface (used to obtain the liquid film thickness).

For primary SE commands and information, please see the documentation: https://kenbrakke.com/evolver/html/evolver.htm

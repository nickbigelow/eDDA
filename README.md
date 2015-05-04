# eDDA
Electron-driven discrete dipole approximation code

This is an electron-driven discrete dipole approximation code called the e-DDA v1.2 [1,2] based off DDSCAT 7.1 [3].

Given a set of dipole points and associated dielectric functions, this code generates a loss probability density for electron energy-loss spectroscopy (EELS) and cathodoluminescence (CL) intensity [4] for a given electron beam trajectory and beam energy. Both internal (beam passes through the target) and aloof (beam does not pass through the target) electron trajectories are permissible in this code. Target rotation functionality is preserved from Draine's original code, which can be used to easily simulate electron tomography experiments.

This code also requires the subroutines:
besseli0.f90
besseli1.f90
besselk0.f90
besselk1.f90
from Numerical Recipes [5].

To install the code simply download DDSCAT v7.1 and move the e-DDA *.f90 files and Makefile into the DDSCAT /src directory.  Compile and run the code exactly as you would with DDSCAT. The only difference is that you must use the supplied ddscat.par file, which contains new information such as the incident electron’s path trajectory and kinetic energy.

Please email us if you have any questions.

[1] N. W. Bigelow, A. Vaschillo, V. Iberi, J. P. Camden, and D. J. Masiello. ACS Nano 6, 7497 (2012).
[2] N. W. Bigelow, A. Vaschillo, J. P. Camden, and D. J. Masiello. ACS Nano 7, 4511 (2013).
[3] B. T. Draine and P. J. Flatau. J. Opt. Soc. Am. A 11, 1491 (1994).
[4] F. J. García de Abajo. Rev. Mod. Phys. 82, 209 (2010).
[5] W. H. Press, B. P. Flannery, S. A. Teukolsky, and W. T. Vetterling. Numerical Recipes. Cambridge University Press, Cambridge (1986).

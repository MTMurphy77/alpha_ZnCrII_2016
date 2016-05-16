# alpha_ZnCrII_2016
Quasar spectra and absorption profile fits associated with Murphy, Malec &amp; Prochaska (2016, MNRAS, submitted).

Read this README, and view/downaload/use the files within this repository, in conjunction with a careful read of the paper itself (Murphy, Malec &amp; Prochaska, 2016, as above).

If you use any of the materials in this repository, please cite the paper.

The paper is available at the following websites, in published or pre-print form:
&ndash; arXiv.org: [LINK TDB]
&ndash; MNRAS: [LINK TDB]
&ndash; NASA/ADS: [LINK TDB]

This repository contains a folder for each quasar spectrum, named using the quasar name (used in the paper) and the spectrograph on which it was observed (Keck/HIRES or VLT/UVES). For example, J0058+0041_HIRES.

Each quasar folder contains a sub-folder which is the nominal redshift of the strong Zn/CrII absorption system fitted in the paper (e.g. 1.072).

Each redshift folder contains the following files:
&ndash; FITS file or files containing the "master spectrum" or "sub-spectra" used in the profile fits to the absorber. The FITS files were all produced using UVES_popler.
&ndash; fit.f13: Absorption profile parameter "guess" file used as input to VPFIT to determine the final parameter values in fit.f26.
&ndash; fit.f18: Record of VPFIT iterations, beginning with the parameters in fit.f13 and proceeding to the final ones in fit.f26
&ndash; fit.f26: Final parameter and 1-sigma uncertainty estimates from VPFIT.

The absorption profile fit was run in VPFIT using the commented-out command in the first line of the fit.f13 file.

The input atomic data file for VPFIT was the MM_VPFIT_2013-11-10.dat file from the <a href="https://github.com/MTMurphy77/MMatomdat">repository</a> associated with <a href="http://adsabs.harvard.edu/abs/2014MNRAS.438..388M">Murphy & Berengut (2014, MNRAS, 438, 388, arXiv:1311.2949)</a>

VPFIT was run using the set-up file in this repository called vp_setup.dat.

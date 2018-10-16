# UVES_SQUAD_DR1
## First data release (DR1) of the UVES Spectral Quasar Absorption Database (SQUAD)

<a href="https://doi.org/10.5281/zenodo.1345974"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.1345974.svg" alt="DOI"></a>

This is a database of 467 high-resolution quasar spectra from the data archive of the [Ultraviolet and Visual Echelle Spectrograph](https://www.eso.org/public/teles-instr/paranal-observatory/vlt/vlt-instr/uves/) (UVES) on the [European Southern Observatory](https://www.eso.org/)'s 8-metre-diameter [Very Large Telescope](https://www.eso.org/public/teles-instr/paranal-observatory/vlt/).

DR1 is documented [in the paper](Paper/paper_accepted_2018-10-16.pdf):  
*Murphy M.T., Kacprzak G.G., Savorgnan G.A.D., Carswell R.F.,
2018, Monthly Notices of the Royal Astronomical Society, accepted, [arXiv:1810.06136](https://arxiv.org/abs/1810.06136)*  
Please cite [the paper](Paper/paper_accepted_2018-10-16.pdf) if you make use of DR1.

The [final DR1 quasar spectra are hosted here](https://data-portal.hpc.swin.edu.au/dataset/uves-squad-dr1) on the [gSTAR Data Management and Collaboration Platform](https://data-portal.hpc.swin.edu.au) (gDMCP). However, this GitHub repository will remain the entrance point to the dataset and can be cited using its DOI, i.e. doi:10.5281/zenodo.1345974*. The [gDMCP data hosting site](https://data-portal.hpc.swin.edu.au/dataset/uves-squad-dr1) contains the following files:
- [**DR1_Final_Spectra.tar.gz:**](https://data-portal.hpc.swin.edu.au/dataset/uves-squad-dr1/resource/8bab4405-4484-4b93-8376-e142409f88a5) Final DR1 spectra of all 467 quasars (Note: File size is 2.1Gb).
- **Individual final spectra** -- *[DR1 quasar name]_Final_Spectrum.tar.gz*: The final spectrum of each quasar is available individually as a gzipped tar file containing the FITS spectrum and the UPL file used in [UVES_popler](https://github.com/MTMurphy77/UVES_popler) to generate it.
- **Individual data reduction files** -- *[DR1 quasar name]_Reduction.tar.gz*: Reduction scripts and all intermediate and final data reduction products for individual quasars as a gzipped tar file. These are required to recreate the final DR1 spectrum of a quasar using the UPL file. Users can also use the UPL file as a starting point for modifying the final spectrum or improving various aspects of the spectrum.


This GitHub repository hosts the following files and folders:
- [**Notes_FITS_Files.txt:**](Notes_FITS_Files.txt) This describes the basic structure of the DR1 final spectra FITS files. **Please read this file if you plan to use the spectra!**
- [**DR1_quasars_master.csv:**](DR1_quasars_master.csv) The master DR1 quasar catalogue. This contains the complete information in Tables 1 and 3 [in the paper](Paper/paper_accepted_2018-10-16.pdf), i.e. the quasar, final spectrum and damped Lyman-alpha system details.
- [**DR1_zlt1.5_ClipMeanComp.fits:**](DR1_zlt1.5_ClipMeanComp.fits) This is the clipped mean composite spectrum of all DR1 quasars with redshifts z<1.5 (and final DR1 spectra), as described in Section 5.2.4 of [the paper](Paper/paper_accepted_2018-10-16.pdf).
- [**Paper folder:**](Paper/) Contains the latest version of the [DR1 paper](Paper/paper_accepted_2018-10-16.pdf), and:
  - [**src sub-folder:**](Paper/src) All the source files that contributed to the paper, including:
    - [**plots_for_paper.ipynb:**](Paper/src/plots_for_paper.ipynb) The Jupyter Notebook used to produce all plots in the paper, including all the analysis behind them.
- [**DLAs folder:**](DLAs/) Further information about the 155 damped Lyman-alpha systems in DR1, including:
  - [**DR1_DLAs.csv:**](DLAs/DR1_DLAs.csv) Catalogue of DLAs extracted from the master catalogue, [DR1_quasars_master.csv](DR1_quasars_master.csv).
  - [**DR1_DLAs.pdf:**](DLAs/DR1_DLAs.pdf) Velocity plots of all DLAs, similar to the example in [the paper](Paper/paper_accepted_2018-10-16.pdf) (figure 14).

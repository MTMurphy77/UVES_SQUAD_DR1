# UVES_SQUAD_DR1
## First data release (DR1) of the UVES Spectral Quasar Absorption Database (SQUAD)

This is a database of 467 high-resolution quasar spectra from the data archive of the [Ultraviolet and Visual Echelle Spectrograph](https://www.eso.org/public/teles-instr/paranal-observatory/vlt/vlt-instr/uves/) (UVES) on the [European Southern Observatory](https://www.eso.org/)'s 8-metre-diameter [Very Large Telescope](https://www.eso.org/public/teles-instr/paranal-observatory/vlt/).

DR1 is documented [in the paper](Paper/paper_submitted_2018-08-10.pdf):  
*Murphy M.T., Kacprzak G.G., Savorgnan G.A.D., Carswell R.F.,
2018, Monthly Notices of the Royal Astronomical Society, submitted*  
This reference will be updated if and when the paper is accepted.  
Please cite [the paper](Paper/paper_submitted_2018-08-10.pdf) if you make use of DR1.

This GitHub repository hosts the following files and folders:
- [**DR1_quasars_master.csv:**](DR1_quasars_master.csv) The master DR1 quasar catalogue. These contain the complete information in Tables 1 and 3 [in the paper](Paper/paper_submitted_2018-08-10.pdf), i.e. the quasar, UVES exposure and damped Lyman-alpha system details.
- [**DR1_zlt1.5_ClipMeanComp.fits:**](DR1_zlt1.5_ClipMeanComp.fits) This is the clipped mean composite spectrum of all DR1 quasars with redshifts z<1.5 (and final DR1 spectra), as described in Section 5.2.4 of [the paper](Paper/paper_submitted_2018-08-10.pdf).
- [**Paper folder:**](Paper/) Contains the latest version of the [DR1 paper](Paper/paper_submitted_2018-08-10.pdf) and:
  - [**src sub-folder:**](Paper/src) All the source files that contributed to the paper, including:
    - [**plots_for_paper.ipynb:**](Paper/src/plots_for_paper.ipynb) The Jupyter Notebook used to produce all plots in the paper, including all the analysis behind them.
- [**DLAs folder:**](DLAs/) Further information about the 155 damped Lyman-alpha systems in DR1, including:
  - [**DR1_DLAs.csv:**](DLAs/DR1_DLAs.csv) Catalogue of DLAs extracted from the master catalogue, [DR1_quasars_master.csv](DR1_quasars_master.csv).
  - [**DR1_DLAs.pdf:**](DLAs/DR1_DLAs.pdf) Velocity plots of all DLAs, similar to the example in [the paper](Paper/paper_submitted_2018-08-10.pdf) (figure 14).
- [**Notes_FITS_Files.txt:**](Notes_FITS_Files.txt) This describes the basic structure of the DR1 final spectra FITS files. *Please read this file if you plan to use the spectra!*

The [final DR1 quasar spectra are currently available here](http://astronomy.swin.edu.au/~mmurphy/data/UVES_SQUAD_DR1). This contains the following files and folders:
- [**DR1_Final_Spectra.tar.gz:**](http://astronomy.swin.edu.au/~mmurphy/data/UVES_SQUAD_DR1/DR1_Final_Spectra.tar.gz) Final DR1 spectra of all 467 quasars (Note: Filesize is 2.1Gb).
- [**Final_Spectra:**](http://astronomy.swin.edu.au/~mmurphy/data/UVES_SQUAD_DR1/Final_Spectra/) Folder containing spectra of individual quasars. The (gzipped) tar file for each quasar contains the final spectrum in FITS format and the UVES_popler log (UPL) file that created it.
- [**Reductions:**](http://astronomy.swin.edu.au/~mmurphy/data/UVES_SQUAD_DR1/Reductions/) Folder containing a (gzipped) tar file for each quasar which contains the data reduction scripts and all intermediate and final data reduction products. These are required to recreate the final DR1 spectrum of a quasar using the UPL file. Users can also use the UPL file as a starting point for modifying the final spectrum or improving various aspects of the spectrum.

*Note: The hosting site of the data will change soon to the [gSTAR Data Management and Collaboration Platform](https://data-portal.hpc.swin.edu.au) (gDMCP). However, this GitHub repository will remain the entrance point to the dataset and can be cited using its DOI, i.e. XXXXXXX.*

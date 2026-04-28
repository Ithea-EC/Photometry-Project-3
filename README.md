# Photometry of M16 (The Eagle Nebula): Project Goals
The objective of this project is to perform an analysis of stars in the M16 star cluster by creating a 2D Gaussian PSF model and radial profile of ten stars in the cluster. After the model fitting, a CMD diagram, which plots magnitude versus color index, is used to analyze the evolutionary stage of the stars in the cluster.

# Table of Contents
* [Methodology](#methodology)
* [Technologies Used](#technologies-used)
* [How to Run](#how-to-run)
* [Project Status](#project-status)
* [AI Contribution](#ai-contribution)
* [Acknowledgements and Sources](#acknowledgements-and-sources)
* [Room for Improvement](#room-for-improvement)
* [Contact](#contact)
<!-- * [License](#license) -->

# Methodology
* Data Acquisition: We downloaded an HST FITS file from the MAST Archive and used DAOStarFinder, a Photutils package, to access data from the file.
  
* Filtering Logic: We used DAOStarFinder to detect the positions of each star and display their data in an organized table.

* Output: For each star, we created a 2D Gaussian PSF model (star cutout) with a corresponding radial profile, and plotted them in a CMD to analyze the evolutionary characteristics of each star in the cluster.

* Organization: Our primary method of organization was through the use of classes. We utilized a class that performs photometry of an object by using FITS file data. In the class, there are five primary functions with the purpose of checking the download status of the FITS file, displaying the image of the object, detecting stars in the object (a star cluster, in this case), extract a cutout of a star (Gaussian PSF fit) from the object to plot a radial profile, and finally, plot the CMD. 

# Technologies Used
* Astropy - Downloading FITS file and image display
* Numpy - Mathematical operations and array usage
* Photutils - Photometry functions
* Matplotlib - Image display and plotting data

# How To Run
1. Clone the repository "Photometry-Project-3".
2. Install dependencies (necessary packages, modules, and any FITS file from the HST MAST Archive).
3. Run the main script once the packages have finished installing. 

# Project Status
Complete

# AI Contribution
There was no AI used in the making of this project. We based most of our code from the sources listed in the Acknowledgements and Sources section. The completion of this project without the use of AI was challenging, but engaging, as our team was able to better our skills in Python coding, as well as fine-tune our problem-solving abilities.

# Acknowledgements and Sources
* https://docs.astropy.org/en/stable/api/astropy.nddata.Cutout2D.html
  - Documentation/code for 2D cutouts of stars.
 
* https://github.com/HorizonIITM/PythonForAstronomy/blob/master/Color-Magnitude-Diagrams/Color-Magnitude%20Diagrams.ipynb
  - Documentation/code for CMD.

* https://spacetelescope.github.io/mast_notebooks/notebooks/SDSS/SDSS_LEGACY_IMAGING_cmd/cmd_diagram.html
  - Potentially useful source for CMD (if FITS data is from SDSS).

* https://www.youtube.com/watch?v=qgJgh0a9qxU (DESI Astro, fantastic resource for many astronomy coding projects!)
  - Documentation/code for DAOStarFinder usage.

* https://photutils.readthedocs.io/en/2.3.0/api/photutils.psf.fit_2dgaussian.html
  - Useful tool for plots used to assess the quality of a 2D Gaussian PSF model.

* https://hst-docs.stsci.edu/acsdhb/chapter-5-acs-data-analysis/5-1-photometry
  - Documentation for header keys to access different filters from FITS files.

* https://photutils.readthedocs.io/en/latest/api/photutils.detection.DAOStarFinder.html
  - General documenation for DAOStarFinder.
  
* https://photutils.readthedocs.io/en/latest/api/photutils.psf.PSFPhotometry.html
  - General photutils documentation.

* https://tingyuansen.github.io/coding_essential_for_astronomers/lectures/lecture20-image-fitting-point-sources-photometry.html
  - Lecture on photometry: point source fitting (Astronomy Data Analysis (ASTRO 1221) at The Ohio State University).
 
# Room for Improvement
- Display radial profiles and 2D Gaussian PSF models one, organized figure. 

# Contact
engum-corral.1@osu.edu
plummer.452@osu.edu 
smedley.48@osu.edu

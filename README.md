# Project Goals
The objective of this tool is to perform an analysis of stars in the M16 star cluster by creating a 2D Gaussian PSF model and radial profile of 10 stars in the cluster. After the model fitting, a CMD diagram is used to analyze the evolutionary status of the stars in the cluster.

# Table of Contents
* [Methodology](#methodology)
* [Technologies Used](#technologies-used)
* [How to Run](#how-to-run)
* [Project Status](#project-status)
* [AI Contribution](#ai-contribution)
* [Acknowledgements and Sources](#acknowledgements-and-sources)
* [Contact](#contact)
<!-- * [License](#license) -->

# Methodology
1. Data Acquisition: We downloaded an HST file from mast and used dao finder to get data from the file.
2. Filtering Logic: We used the package daofinder that finds all the stars in the cluster and gives data about them in a table.
3. Output: Results take the magnitude and display them in a CMD graph to analyze what evolutionary type of stars live in this cluster.
4. Organization: We created a class that creates the Gaussian PSF fit, and the radial profile and graphes them. We just give the specific star x and y coords and initialize the class to display the Gaussian PSF fit and radial profile.

# Technologies Used
* Astropy
* Numpy  
* Photutils
* Matplotlib 

# How To Run
1. Clone the repo
2. Install dependencies
3. Run the main script

# Project Status
Complete

# AI Contribution
There was no AI used in the making of this project.

# Acknowledgements and Sources
https://docs.astropy.org/en/stable/api/astropy.nddata.Cutout2D.html
https://github.com/HorizonIITM/PythonForAstronomy/blob/master/Color-Magnitude-Diagrams/Color-Magnitude%20Diagrams.ipynb
https://spacetelescope.github.io/mast_notebooks/notebooks/SDSS/SDSS_LEGACY_IMAGING_cmd/cmd_diagram.html
https://www.youtube.com/watch?v=qgJgh0a9qxU (DESI Astro, fantastic resource!)
https://photutils.readthedocs.io/en/2.3.0/api/photutils.psf.fit_2dgaussian.html
https://hst-docs.stsci.edu/acsdhb/chapter-5-acs-data-analysis/5-1-photometry
https://photutils.readthedocs.io/en/latest/api/photutils.detection.DAOStarFinder.html
https://photutils.readthedocs.io/en/latest/api/photutils.psf.PSFPhotometry.html
https://tingyuansen.github.io/coding_essential_for_astronomers/lectures/lecture20-image-fitting-point-sources-photometry.html

# Contact
engum-corral.1@osu.edu
plummer.452@osu.edu 
smedley.48@osu.edu

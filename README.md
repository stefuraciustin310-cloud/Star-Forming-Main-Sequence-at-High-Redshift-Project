# Star-Forming-Main-Sequence-at-High-Redshift-Project
This project analyzes the Star-Forming Main Sequence (SFMS) of galaxies at high redshift (z = 3 and z  = 5) using spectroscopic and photometric data from the James Webb Space Telescope (JWST).
The goal is to estimate star formation rates (SFRs) and stellar masses for a sample of galaxies and investigate how the SFMS evolves across time.
The analysis uses public JWST data and applies simplified and empirical methods to extract physical galaxy properties from noisy, high-redshift observations.

Data:

DAWN JWST Archive 

    -NIRSpec - JADES survey
    
    -NIRCam photometry
    
Methodology:

    -Spectral Data Processing
    
        Downloaded JWST NIRSpec spectra in FITS format
        
        Extracted wavelength, flux density, and flux uncertainty data
        
        Visualized spectra in observed-frame wavelength space
        
        Identified the expected location of the Hα emission line using galaxy redshifts
        
    -Star Formation Rate Estimation
    
        Extracted the Hα emission line region from each spectrum
        
        Modeled emission lines using Gaussian fitting
        
        Integrated the Gaussian fits to obtain Hα fluxes
        
        Converted Hα luminosities to star formation rates using the Kennicutt & Evans (2012) relation
        
        Uncertainties were estimated by combining measurement errors with the intrinsic scatter of the Hα–SFR relation.
        
    -Stellar Mass Estimation
    
        Cross-matched spectroscopic targets with JADES photometric catalogs
        
        Selected photometric bands corresponding to rest-frame 1500 Å
        
        Converted observed flux densities to AB magnitudes and absolute magnitudes
        
        Estimated stellar masses using the empirical M*–MUV relation from Tacchella et al. (2018)
        
        Uncertainties include photometric errors and the intrinsic scatter of the mass–luminosity relation.
        
    -Analysis and Visualization
    
        Produced tables and histograms of stellar mass distributions
        
        Created stellar mass versus SFR diagrams for different redshift bins
        
        Compared results with literature SFMS relations from Popesso et al. (2022)
        
        Assessed sources of uncertainty and methodological limitations
Tools and Technologies:
  
Programming language: Python
  
Libraries: NumPy, Pandas, SciPy, Matplotlib

Data formats: FITS

Environment: Jupyter Notebook

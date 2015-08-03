This package of MATLAB routines with accompanying GUI allows scientific users to measure the 3D location of single molecules when using the double-helix point spread function (DH-PSF) widefield microscope.

**Features**
  * Double-Gaussian estimator is calibrated via an axial scan of bright immobile fluorescent emitters (e.g. beads).
  * Template-matching and double-helix recognition algorithm is calibrated via setting an image correlation threshold against single-molecule data.
  * Tiff stacks of SM images are analyzed using template matching followed by double-Gaussian fitting to extract estimates of the molecule positions.
  * The motion/drift of fiduciaries (e.g. fluorescent beads) during an experiment can tracked and removed form SM localization data.
  * 3D localization data can be exported to .csv format for post-processing and visualization.
  * Basic 3D scatterplot and 2D _z_-projection histogram visualizations are included.

| **Contents** |
|:-------------|
|              |


# Getting started #

## System requirements ##
[MATLAB](http://www.mathworks.com/products/) and its associated image processing, optimization, statistics, and wavelet toolboxes are required. The code has been tested with MATLAB R2011b and R2012b. No known issues exist with other versions of MATLAB, but some built-in functions (e.g. `fft2`, `imread`) may exhibit degraded performance in older versions of MATLAB.

## Downloading and installing ##
The source code can be downloaded via the instructions below. No installation is needed; simply place the source code in your MATLAB path and run `easy_dhpsf` from the MATLAB command line.  As usual, read the documentation first!

### Stable version ###
**Note: Google has recently disabled the "downloads" functionality of Google code. Please use our [Mercurial repository](#Latest_version.md) to keep your software up to date.**

A stable version of the source code is available as a zip archive. Download it from the [featured downloads](https://code.google.com/p/easy-dhpsf/downloads/list?q=label:Featured) list at left.

  * Version 1.02: Fixed bugs in f\_fitSMs and f\_concatSMfits

  * Version 1.01: Streamlined f\_calDHPSF

  * Version 1.0: Initial build

### Latest version ###
Please use Mercurial to keep up to date with the latest features and bug-fixes.
```
hg clone https://your-google-username@code.google.com/p/easy-dhpsf/
```
A great Windows client for Mercurial is [TortoiseHg](http://tortoisehg.bitbucket.org/).



# Documentation #
There are two versions of the documentation available.
  * Lew, M. D.`*`,  von Diezmann, A. R. S.`*`,  and Moerner, W. E. “Easy-DHPSF open-source software for three-dimensional localization of single molecules with precision beyond the optical diffraction limit” _Protocol Exchange_ (2013). DOI: [10.1038/protex.2013.026](http://dx.doi.org/10.1038/protex.2013.026)
  * PDF located in the [featured downloads](https://code.google.com/p/easy-dhpsf/downloads/list?q=label:Featured) list at left

<a href='Hidden comment: 
*** NOTE: Do not change the "Sample single-molecule DH-PSF data" heading below!! It is directly hyperlinked from the Protocol Exchange article!! ***
'></a>
## Sample single-molecule DH-PSF data ##
The sample files entitled "MT\_sample\_data" can be found in the [Downloads](https://code.google.com/p/easy-dhpsf/downloads/list) section. This data was published in:
> Lee, H. D.`*`, Sahl, S. J.`*`, Lew, M. D. & Moerner, W. E. The double-helix microscope super-resolves extended biological structures by localizing single blinking molecules in three dimensions with nanoscale precision. _App. Phys. Lett._ **100**, 153701 (2012). `[`[link](http://dx.doi.org/10.1063/1.3700446)`]`


# Program history and development team #
This code grew out of a desire to automate the fitting process for DH microscope data as a "Digital Image Processing" class project. Since then, features have been added and bugs have been fixed to make it ready for us by others with MATLAB experience.

  * **Version 1.0**, _2012-present_: Matthew D. Lew, Alexander R. S. von Diezmann, Andreas Gahlmann, Mikael P. Backlund, W. E. Moerner
> Featured in:
    1. Gahlmann, A. _et al_. Quantitative multicolor subdiffraction imaging of bacterial protein ultrastructures in 3D. _Nano Lett._ (2013). `[`[link](http://dx.doi.org/10.1021/nl304071h)`]`
  * **Version 0.5**, _Summer 2010-2011_: Matthew D. Lew, Steven F. Lee, Steffen J. Sahl, Alex Chang, W. E. Moerner
> Featured in:
    1. Lew, M. D.`*`, Lee S. F.`*`, _et al_. Three-dimensional superresolution colocalization of intracellular protein superstructures and the cell surface in live _Caulobacter crescentus_. _Proc. Natl. Acad. Sci. USA_ **108**, E1102-E1110 (2011). `[`[link](http://dx.doi.org/10.1073/pnas.1114444108)`]`
    1. Lee, H. D.`*`, Sahl, S. J.`*`, Lew, M. D. & Moerner, W. E. The double-helix microscope super-resolves extended biological structures by localizing single blinking molecules in three dimensions with nanoscale precision. _App. Phys. Lett._ **100**, 153701 (2012). `[`[link](http://dx.doi.org/10.1063/1.3700446)`]`
  * **Version 0.1**, _Spring 2010_: Matthew D. Lew and Scott S. Hsieh
> [EE 368 Digital Image Processing class project](http://www.stanford.edu/class/ee368/Project_10/)
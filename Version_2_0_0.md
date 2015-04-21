## Spectral Indices Version 2.0.0 Release Notes ##
Release Date: June 9, 2014

### Downloads ###

**Spectral indices source code - available via the [spectral-indices Google Projects Source](https://code.google.com/p/spectral-indices/source/checkout) link**

  * Non-members may check out a read-only working copy anonymously over HTTP.
  * svn checkout http://spectral-indices.googlecode.com/svn/releases/version_2.0.0 spectral-indices-read-only

### Installation ###
Same installation instructions as for Version 1.0.0 with the addition of the ESPA raw binary libraries and tools in the [espa\_common Google Project](https://code.google.com/p/espa-common/).  The user will need to build the src/raw\_binary code to create the libraries used for building the current version of the spectral indices application.

### Dependencies ###
Same dependencies as for Version 1.0.0 with the addition of the ESPA raw binary libraries and tools in the [espa\_common Google Project](https://code.google.com/p/espa-common/).  The user will need to build the src/raw\_binary code to create the libraries used for building the current version of the spectral indices application.

### Data Preprocessing ###
This version of the spectral indices application requires the input Landsat products to be in the ESPA internal file format.

### Data Postprocessing ###
After compiling the espa-common raw\_binary libraries and tools, the convert\_espa\_to\_gtif and convert\_espa\_to\_hdf command-line tools can be used to convert the ESPA internal file format to HDF or GeoTIFF.  Otherwise the data will remain in the ESPA internal file format, which includes each band in the ENVI file format (i.e. raw binary file with associated ENVI header file) and an overall XML metadata file.

### Associated Scripts ###
Same scripts as for Version 1.0.0, updated for 2.0.0

### Verification Data ###

### User Manual ###

### Product Guide ###


## Changes From Previous Version ##
#### Updates on June 9, 2014 - USGS EROS ####
  * src
    1. Modified to process data in the ESPA internal file format vs the previous HDF file format.  The XML file is passed in as input to this application.  Added command-line flag (--toa) to specify whether the TOA or the SR bands should be used for computing the spectral indices.

  * scripts
    1. Modified the script to support changes to the command-line parameters for the XML input and the additional command-line flag.
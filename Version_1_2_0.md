## Spectral Indices Version 1.2.0 Release Notes ##
Release Date: November 13, 2013

### Downloads ###

**Spectral indices source code - available via the [spectral-indices Google Projects Source](https://code.google.com/p/spectral-indices/source/checkout) link**

  * Non-members may check out a read-only working copy anonymously over HTTP.
  * svn checkout http://spectral-indices.googlecode.com/svn/tags/version_1.2.0 spectral-indices-read-only

### Installation ###
Same installation instructions as for Version 1.0.0

### Dependencies ###
Same dependencies as for Version 1.0.0

### Associated Scripts ###
Same scripts as for Version 1.0.0, updated for 1.2.0.

### Verification Data ###

### User Manual ###

### Product Guide ###


## Changes From Previous Version ##
#### Updates on November 13, 2013 - USGS EROS ####
  * src
    1. Modified the application to write out all the vegetation indices (NDVI, EVI, SAVI, MSAVI) to the same output file, containing multiple bands.  As with previous releases, only the user-specified indices will be written.  And, the other indices (NBR, NBR2, NDMI) are still written to their own output file as single bands.
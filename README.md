## Introduction
The purpose of this notebook is to provide some examples of how to use the WebbPSF trending API for JWST WFS&C Data.  Code excerpts and text extracted from: https://webbpsf.readthedocs.io/en/latest/jwst_measured_opds.html

### Defining terms
For more information on JWST Acronyms and abbreviations please see: https://jwst-docs.stsci.edu/jwst-acronyms-and-abbreviations#gsc.tab=0

For more information on JWST Wavefront Sensing and Control: https://jwst-docs.stsci.edu/jwst-observatory-hardware/jwst-wavefront-sensing-and-control#gsc.tab=0

## Installing WebbPSF and required data files
Follow installation instructions on WebbPSF:
https://webbpsf.readthedocs.io/en/latest/installation.html

If you install via pip or manually, you must install the data files yourself.

Files containing such information as the JWST pupil shape, instrument throughputs, and aperture positions are distributed separately from WebbPSF. To run WebbPSF, you must download these files and tell WebbPSF where to find them using the WEBBPSF_PATH environment variable.

  1. Download the following file: [webbpsf-data-LATEST.tar](https://stsci.box.com/shared/static/qxpiaxsjwo15ml6m4pkhtk36c9jgj70k.gz) [approx. 70 MB]

  2. Untar webbpsf-data-LATEST.tar.gz into a directory of your choosing.

  3. Set the environment variable WEBBPSF_PATH to point to that directory. e.g.
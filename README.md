Genome structure analysis scripts
=================================

This repository contains an ipython notebook script which demonstrates the
following:

Calculation of "Void" regions in population Hi-C data - a small proportion of
the sequence with unusual numbers of contacts that is excluded from structural
analyses.

Calculation of A/B chromosome compartments using population Hi-C data using a
simple k-means clustering of the covarience matrix of the observed to expected 
contact ratio.

Calculation of spatial density enrichment whereby 3D co-localisation of two data
tracks on a genome structure is compared to a random/null hypothesis where
sequence positions of the data are circularly permuted (thus preserving sequence
relationships but sampling diffferent structural conformations). This analysis
allows the degree of spatial clustering to be assessed above what is expected
from relative sequence positioning of the data, i.e it removes the effect of
sequence clustering.

Each of the above is achieved by a separate function within the larger script
which also contains all of the necessary utility functions.

Installation
============

After following the installation instructions, the notebook can be run with the
command `jupyter-notebook` in the repository folder.

Python Packages
---------------

Dependencies are *SciPy*, *NumPy*, *matplotlib* and *Cython*. These are all
available through pip, and in most distributions' package managers. To view the
notebook, a web browser is required.

Jupyter
-------

Jupyter can be installed using `pip install jupyter`, for either Python3 and
Python2.

The notebook is written in Python2, so the Python2 Jupyter kernel must be
installed: `pip2 install ipykernel` followed by `python2 -m ipykernel install`.

*Note:* it might be necessary to explicitly select the Python2 kernel from the
`Kernel` menu when running the notebook.

Data Files
----------

The script requires the demonstration data (available as a .tar.gz archive) to
be extracted into the same directory as the notebook script, but otherwise the
material is self-contained. 

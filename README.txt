Genome structure analysis scripts
---------------------------------

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
which also contains all of the necessary utility functions. There are no
dependencies beyond the usual SciPy bundle (so including NumPy and matplotlib).

The script requires the demonstration data (available as a .tar.gz archive) to
be extracted into the same directory as the notebook script, but otherwise the
material is self-contained. 

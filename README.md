# CONJ models - Models for detection of conjugative and mobilisable plasmids

This set of MacSyFinder's models are dedicated to the detection of conjugative and mobilisable plasmids.
The conjugative T4SS that can be detected are:

- T4SS_typeG
- T4SS_typeF
- T4SS_typeC
- T4SS_typeB
- T4SS_typeI
- T4SS_typeT
- T4SS_typeFA
- T4SS_typeFATA

Mobilisable plasmids detected will be described as:

- MOB

This set of models is an updated version of those published in 2017 by Cury, et al. The models are now compatibles with **MacSyFinder version 2**.

## Installation and Usage with MacSyFinder

First, the `macsyfinder` program should be [installed](http://macsyfinder.readthedocs.io/en/latest/). This will also install the `macsydata` tool that enables to easily install this package of MacSyFinder models from this repository.


The basic commands to run are then:

    macsydata install CONJScan_plasmids


to install the CONJScan plasmids package.

    macsyfinder --db-type ordered_replicon \
		--sequence-db myproteins.fasta \
		--models CONJScan_plasmids system 		


to run the search on your favorite organism's genome, where `system` is one or multiple systems listed above, or `all` to search for all the above listed systems
(see [MacSyFinder's documentation](http://macsyfinder.readthedocs.io/en/latest/)).


It has to be noted that to ensure the highest annotation specificity, it is recommended to search for **all** systems in the package at once.


## References

- Jean Cury, Marie Touchon, Eduardo P. C. Rocha,
  Integrative and conjugative elements and their hosts: composition, distribution and organization.
  Nucleic Acids Research, Volume 45, Issue 15, 6 September 2017, Pages 8943–8956.
  [doi: 10.1093/nar/gkx607](https://doi.org/10.1093/nar/gkx607)

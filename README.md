# Singularity Recipe for ete3

This repo contains recipes to run [ete3](http://etetoolkit.org/)
within a [Singularity](http://singularity.lbl.gov/) container, which can be built 
using [Singularity Hub](https://singularity-hub.org/)

Versions:

* 3.1.1 - ete3 v3.1.1 from anaconda installed on Fedora

## How to Use:

Run example:

singularity run shub://ResearchIT/ete3 build check

## Alternative method:
use the provided bash wrapper and module file to use the singularity container like a standard module
(this assumes you have a singularity/2.4 module)

e.g.

module load ete3
ete3 build check 

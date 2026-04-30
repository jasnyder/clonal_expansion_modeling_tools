[![DOI](https://zenodo.org/badge/1025014211.svg)](https://doi.org/10.5281/zenodo.19922835)

This is a set of tools to support the simulations and analysis in the paper _Mathematical modeling of JAK2V617F clonal expansion in a general population cohort_, by Jordan Snyder et al.

# Installation
Install this package using `pip`, either locally or via PyPI.

## Locally
1. Clone this repository in an empty directory
2. Navigate to the repsitory and run
```bash
pip install .
```
optional: add the `-e` flag if you would like to edit the code and have changes available on next kernel restart without having to re-install the package.

## From PyPI
Run
```bash
pip install clonal_expansion_modeling_tools
```

# Usage
This package provides two subpackages: `gesus_routines`, focused on cleaning and loading data, and `moran_models`, focused on simulation and parameter estimation for the [Moran process](https://en.wikipedia.org/wiki/Moran_process), including parsing files output from Bayesian estimation using [ApproxBayes.jl](https://github.com/marcjwilliams1/ApproxBayes.jl)

To use the functions provided in this package, do
```python
from clonal_expansion_modeling_tools import gesus_routines, moran_models
```

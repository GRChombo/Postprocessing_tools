# YTAnalysis
This folder contains a set of tools for running analysis on the HDF5 files generated by GRChombo. All of the scripts run in parallel with near perfect scaling as long as the number of cores used = number of files. These have been recently refactored and updated, however have not been retested after this process. Use at your own risk and please issue PRs with any corrections. Note as well these files use [Black](https://github.com/psf/black) for formatting and [PyFlakes](https://pypi.org/project/pyflakes/) for linting.

# Requirments
Check out the requirements.txt file for the list of packages required. Note that these scripts were originally written for python2.7 and have since been refactored for python3 compatability.

## parallel_convergence.py
Used for creating convergence tests. Note that this is tricky to use, and requires some _fiddling_.

## parallel_energy.py
Calculates potential, gradient and kinetic energy.

## parallel_L.py
Calculates L2M and L2H.

## parallel_phi.py
Calculates the min and max of phi.

## parallel_pictures.py
Used for creating slice plots (default is to slice along the z-axis)

## parallel_Psi4.py
Decomposition of Psi4 into spin weighted spherical harmonics. This is largely based off an older script by Thomas Helfer.

## parallel_radius.py
Script to calculate radius of an axion star. See the appendix of this [paper](https://arxiv.org/abs/1806.09367) for more information.
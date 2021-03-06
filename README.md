[ ![Documentation](https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://halem.readthedocs.io)
[ ![License: MIT](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/TUDelft-CITG/HALEM/blob/master/LICENSE.txt)
[ ![DOI](https://zenodo.org/badge/184024759.svg)](https://zenodo.org/badge/latestdoi/184024759)

[ ![CircleCI](https://circleci.com/gh/TUDelft-CITG/HALEM.svg?style=svg&circle-token=64796bff34a56507bad599a6cec980b7b8be0bb9)](https://circleci.com/gh/TUDelft-CITG/HALEM)
[ ![Coverage](https://oedm.vanoord.com/proxy/circleci_no_redirect/github/TUDelft-CITG/HALEM/master/latest/ddf5d3b409fbb3e3aa368be6b0b0907c53c40a87/tmp/artifacts/coverage.svg)](https://oedm.vanoord.com/proxy/circleci_no_redirect/github/TUDelft-CITG/HALEM/master/latest/ddf5d3b409fbb3e3aa368be6b0b0907c53c40a87/tmp/artifacts/index.html)
[ ![BlackFormatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

# HALEM

**H**ydrodynamic **A**lgorithm for **L**ogistic **E**nhancement **M**odule: route optimisation in dynamic currents.

Documentation can be found [here](https://halem.readthedocs.io).

## Features

This package contains route optimization for given currents. The following features are taken into account in this version:

* Spatial varying currents
* Temporal changing currents
* Variable shipping velocity
* minimal water depth
* Squad

Does not take into account:

* Inertial behavior of the ship

Different routes that can be optimized are:

* Shortest route (halem.HALEM_time)
* Fastest route (halem.HALEM_space)
* Cheapest route route (halem.HALEM_cost)
* Cleanest route (halem.HALEM_co2)

## Implementation

This package can be used to find an optimal route in dynamic flowfields. For simulation purposes it can be implemented into [OpenCLSim](https://github.com/TUDelft-CITG/OpenCLSim). For an introduction on how to do so please check Jupyter Notebook [number 08](https://github.com/TUDelft-CITG/OpenCLSim-Notebooks/blob/master/notebooks/Example%2008%20-%20Basic%20hopper%20operation%20on%20route%20with%20halem.ipynb) of the OpenCLSim examples or the [tests](https://github.com/TUDelft-CITG/HALEM/blob/master/tests/test_openclsim.py).

## Installation

The Package can be installed using pip. Type following code in the python command prompt:

``` bash
pip install halem
```

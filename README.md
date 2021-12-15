# Microtubule dynamics simulation
Simulation of microtubule growth dynamics in the presence and absence of physical obstacles.

Work done by:
- Simulation code: Florian Huber and Maurits Kok
- Experiments run by: Maurits Kok and Svenja-Marei Kalisch
- Marileen Dogterom

## Reference / citation
You can read more about this simulation in:  
[Kok, Huber, Kalisch, Dogterom, 2021, bioRxiv, DOI: 10.1101/2021.12.07.471417](https://doi.org/10.1101/2021.12.07.471417)

Please also cite this article if use the present code or results. Thanks!


## Simulation code
[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/florian-huber/mtdynamics/Build)](https://img.shields.io/github/workflow/status/florian-huber/mtdynamics/Build)
[![Liscence](https://img.shields.io/github/license/florian-huber/mtdynamics)](https://github.com/florian-huber/mtdynamics)
[![PyPI](https://img.shields.io/pypi/v/mtdynamics?color=blue)](https://pypi.org/project/mtdynamics/0.1.1/)
[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)

The full simulation code used to produce the results as published in [coming soon] is provided.\ in this repository.  
The code consits of the main simulation code (**simulation_main.py** and **simulation_functions.py**). Simulation parameters are specified in **simulation_parameters.py**. Functions for plotting the results are provided in **plotting_functions.py**.

### Requirements
Python version 3.6 or higher.

### Installation
If you work with Anaconda you can create an own environment for ``mtdynamics`` by running the following commands:

```
# install mtdynamics in a new virtual environment to avoid dependency clashes
conda create --name mtdynamics python=3.7
conda activate mtdynamics
pip install mtdynamics
pip install jupyter  # Optional, if you want to run jupyter notebooks from this environment
conda install -c anaconda pywin32  # Optional, if you run into win32api error (e.g. when using Python 3.8)
```

Or simply install mtdynamics in your already existing environment:
```
pip install mtdynamics
```

## Runing the simulation
Jupyter notebook(s) are provided to illustrate how to run the simlation. They can be found in the folder ``\notebooks``.

## Making a new release

To create release you need write permission on the repository.

1. Check author list in `citation.cff` file.
1. Update version in ``setup.py`` and ``CHANGELOG.md``.
1. Update the `CHANGELOG.md` to include changes made.
1. Goto [GitHub release page](https://github.com/florian-huber/mtdynamics/releases)
1. Press draft a new release button
1. Fill version, title and description field
1. Press the Publish Release button

A GitHub action will run which will publish the new version to [pypi](https://pypi.org/).

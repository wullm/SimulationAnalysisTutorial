# ExGal Summer School Tutorial: Analyzing simulations

In this tutorial, you will gain experience with analyzing cosmological N-body simulations. The tutorial consists of three parts, each chapter introducing you to a different set of codes.

Before getting started, we need to set up an environment and install the necessary packages.

## Setting up a virtual environment

Once you're logged into cosma, run the following commands in the terminal. This will create a new virtual environment, providing us with a clean workspace to install all the necessary python packages.

```
mkdir ~/venvs && cd ~/venvs
python -m venv my_environment
```

To activate the environment run

```
source my_environment/bin/activate
```

Next, we want to make the environment available for Jupyter Notebook.

```
pip install ipykernel
python -m ipykernel install --user --name=my_environment
```

(In case you want to remove an environment from Jupyter, you could use ``jupyter kernelspec uninstall my_environment``. To delete the environment altogether, you can simply remove the corresponding directory.)

## Required packages

You will need to install the following Python packages

```
pip install pylians
pip install pynbody
pip install swiftsimio
pip install swiftgalaxy
pip install h5glance
```

## Connecting to Jupyter

To connect to Jupyter Hub, run the following command on your local machine

```
ssh -L localhost:8443:login8b:443 USER@login8b.cosma.dur.ac.uk
```

replacing ``USER`` with your cosma username. You can then access Jupyter via https://localhost:8443/. See https://cosma.readthedocs.io/en/latest/jupyter.html for further instructions. This page also contains instructions for running Jupyter on a compute node.


# ExGal Summer School Tutorial 1: Analyzing simulations

In this tutorial, you will gain some experience with the basic analysis of cosmological N-body simulations. The tutorial consists of three parts, each chapter introducing you to a different set of codes.

Before getting started, we need to set up an environment and install the necessary packages.

## Setting up a virtual environment

Once you're logged into cosma, run the following commands in the terminal. This will create a new virtual environment, providing us with a clean workspace to install all the necessary python packages.

```
mkdir ~/venvs && cd ~/venvs
python -m venv my_environment
```

To activate, the environment run

```
source my_environment/bin/activate
```

Next, we want to make the environment avaiable for Jupyter Notebook.

```
pip install ipykernel
python -m ipykernel install --user --name=my_environment
```

(In case you want to remove an environment from Jupyter, you could use ``jupyter kernelspec uninstall my_environment``. To delete the environment altogether, you can simply remove the corresponding directory.)

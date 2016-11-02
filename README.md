# Bayesian Election Forcasting using PyMC3

PyMC3 implementation of Drew Linzer’s dynamic Bayesian election forecasting model, converted from original Stan implementation by Pierre-Antoine Kremp.

[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org:/repo/fonnesbeck/election_pycast)

## Running model remotely

You can run this model in a web browser using Jupyter Notebooks hosted on [Binder](http://mybinder.org), without having to install anything on your local machine. To run the model on Binder, click on the **Launch binder** button above.

## Running model locally

The election_pycast model requires Python 3 be installed on your system. Perhaps the easiest way to get a feature-complete version of Python on your system is to install the [Anaconda](http://continuum.io/downloads.html) distribution by Continuum Analytics. Anaconda is a completely free Python environment that includes includes almost 200 of the best Python packages for science and data analysis. Its simply a matter of downloading the installer (either graphical or command line), and running it on your system.

Once Python is installed, use Git to clone this repository to your machine:

    git clone https://github.com/fonnesbeck/election_pycast.git

If you are not familiar with Git and GitHub, you can simply download the zip file of the repository at the top of the main repository page.

Then, move to the directory created by the clone/zip file:

    cd election_pycast

and install everything using `conda`:

    conda env create -f environment.yml
    
This will create an **environment** called `election` that includes the packages required to run the model.   This environment can be enabled by running:

    source activate election
    
from a macOS or Linux machine, or:

    activate election
    
from a Windows machine.

With your environment activated, you can start Jupyter in your working directory:

    jupyter notebook
    
Select the `Election2016.ipynb` notebook to open the model.
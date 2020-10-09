# Jupyter Notebooks for R

This folder contains a Jupyter Notebook with R code examples. 

The file can be open either on:
- An online Jupyter server with R support. Recommended [Kaggle](https://www.kaggle.com/)
- A local Jupyter instance with R support.


## Installing and configuring a local Jupyter Notebook server with R support

These instructions are an excerpt for `conda` from the links provided. Detailed instructions, and instructions for `pip` can be found in the links.

1. [Install Anaconda](https://docs.anaconda.com/anaconda/install/)
2. Install an R kernel for Jupyter, [IRkernel](https://irkernel.github.io/installation/)
```R
install.packages("IRkernel")
```
3. Create and active a new [conda R environment](https://docs.anaconda.com/anaconda/user-guide/tasks/using-r-language/) with all the r-essentials conda packages and other specific (CRAN) packages that you need
```bash
conda create -n r_env r-base r-essentials r-foreach r-doParallel
conda activate r_env
# List the packages in the environment
conda list
```

You are ready to start [using the R programming language in Jupyter Notebook](https://docs.anaconda.com/anaconda/navigator/tutorials/r-lang/)


## Optional. Installing and managing Jupyter Notebook extensions

1. Install jupyter client
```bash
sudo apt install jupyter-client
```

2. [Install jupyter_contrib_nbextensions](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/install.html)
```bash
conda install -c conda-forge jupyter_contrib_nbextensions
# Install javascript and css files
jupyter contrib nbextension install --sys-prefix
```

3. [Install jupyter_nbextensions_configurator](https://github.com/Jupyter-contrib/jupyter_nbextensions_configurator)
```bash
conda install -c conda-forge jupyter_nbextensions_configurator
```

## Extra. Conversion between .Rmd and .ipynb
An RMarkdown content manager for Jupyter Notebook: [ipymd](https://github.com/grst/ipymd)

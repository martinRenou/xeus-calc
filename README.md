# xeus-calc

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/QuantStack/xeus-calc/master?filepath=notebooks/Xeus-calc.ipynb)
[![Travis](https://travis-ci.org/QuantStack/xeus-calc.svg?branch=master)](https://travis-ci.org/QuantStack/xeus-calc)
[![Appveyor](https://ci.appveyor.com/api/projects/status/jh45g5pj44jqj8vw?svg=true)](https://ci.appveyor.com/project/QuantStack/xeus-calc)

Calculator as a Jupyter Kernel implemented with Xeus

## Usage

Launch the Jupyter notebook with `jupyter notebook` or Jupyter lab with `jupyter lab` and launch a new notebook by selecting the **xeus-calc** kernel.

**Basic calculation**:

![Basic calculation](xeus-calc2.gif)



## Installation


To ensure that the installation works, it is preferable to install `xeus` in a fresh conda environment. It is also needed to use a [miniconda](https://conda.io/miniconda.html) installation because with the full [anaconda](https://www.anaconda.com/) you may have a conflict.

The safest usage is to create an environment named `xeus-calc-env` within your miniconda installation

```bash
conda create -n xeus-calc-env
conda activate xeus-calc-env
conda install -c conda-forge xeus
```


Once you have installed ` xeus ` ,the  ` xeus-calc ` project is quite easy to install, you have to clone the repository, and run the following command lines :


```bash
mkdir build
cd build
cmake -D CMAKE_INSTALL_PREFIX=$CONDA_PREFIX ..
make
make install
```

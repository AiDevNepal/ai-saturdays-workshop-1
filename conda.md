# Conda 

## Introduction
It is an environment management system for Python (also can be for other language) that is packaged with popular modules and libraries
for python for doing data science and machine learning.  

A conda environment has following stuff available:
1. numpy
2. pandas
3. matplotlib
4. jupyter notebook

--------

## Installation - Linux

### Download the linux installer
Download the shell script (installer) for linux from the link:  
[https://www.anaconda.com/download/#linux](https://www.anaconda.com/download/#linux)  
Python version **3+** is recommended.

### Install using the shell script
Open your terminal and run the script
```bash
bash anaconda_script_name.sh
```

Here, **anaconda_script_name** will be according to your download.


### Add the conda to system path
By default, the installation script should add the conda to the system path.  

If not, then you have to add it to **bashrc** file as:

- open **.bashrc** existing in your home directory
- export the **path** variable as:

```bash
export PATH=${PATH}:"path_to_conda_bin"
```

--------

## Installation - Windows

### Download the installer for windows
Download the graphical installer for windows.  
[https://www.anaconda.com/download/#windows](https://www.anaconda.com/download/#windows)  

Make sure you choose the right architecture (32-bit/64-bit) according to your device.

### Run the installer
Make sure you choose **add to system path** or similar box to add the conda command to system.

--------

## General Usage

### Create a new conda environment
You can create a new conda environment by using the command:
```bash
conda create --name env_name
```

where, **env_name** can be any name without spaces. Eg:
```bash
conda create --name workshop-1
```

### Switch to existing environment
The environment if available can be activated as:
```bash
source activate workshop-1
```

Once the environment is activated, the command prompt shows the environment's name inside small brackets like:
```bash
(workshop-1) user:~$ 
```

### Confirm the existing modules/libraries
Once inside the environment, open python shell by tying `python` and try importing the modules:
```bash
>>> import numpy as np
>>> import pandas as pd
>>> import matplotlib.pyplot as plt
```

If conda's installation and setup was successful, there'd be no errors importing those modules.


### Deactivate the environment
Run the command:
```bash
source deactivate
```

### Run Jupyter Notebook
Inside the activated conda environment, run the command:
```bash
jupyter notebook
```

The notebook will start at `localhost:8888`. So, make sure you open your browser and hit that url.

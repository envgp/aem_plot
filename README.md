**[summary](#summary) | [prerequisites](#prerequisites) | [setup](#setup) | [resources](#resources) | [license](#license)**

# Plotting a Resistivity Model from Airborne Electromagnetic Data

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/simpeg/transform-2021-simpeg/HEAD)
[![License](https://img.shields.io/github/license/simpeg/transform-2021-simpeg.svg)](https://github.com/simpeg/transform-2021-simpeg/blob/master/LICENSE)

|         | Info |
|--------:|:-----|
| When    | Wednesday, February 16 • 16:00-17:00 pm PST |
| YouTube | TBA |
| conda environment  | `aem_plot` |
| Slides  | [AEM Plot presentation](https://bit.ly/aem_plot_slides) |


## Prerequisites

**Software**

* Some knowledge of Python is assumed.
* All coding will be done in Jupyter notebooks. I'll explain how they work
  briefly but it will help if you've used them before.
* We'll use [numpy](https://numpy.org/), [matplotlib](https://matplotlib.org/), and
  [ipywidgets](https://ipywidgets.readthedocs.io/)
  You don't need to be an expert in these tools but some familiarity will help.

**Airborne Electromagnetic Mehtod**

* XXX
* As a motivating example, XXX

## Usage

There are a few things you'll need to follow the tutorial:

1. A working Python installation ([Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
2. The SimPEG *conda environment* installed
3. A web browser that works with Jupyter
   (basically anything except Internet Explorer)

To get things setup, please do the following.

**Windows users:** When you see "*terminal*" in the instructions,
this means the "*Anaconda Prompt*" program for you.

### Step 1: Python

**Follow the general instructions for installing Anaconda:** https://www.youtube.com/playlist?list=PLgLft9vxdduAW-jmhYqXvtfGYJS6v2FjM

This will get you a working Python 3 installation with the `conda` package
manager. If you already have one, you can skip this step.

### Step 2: Download the AEM Plot tutorials

To access the notebooks, there are 3 options (in order of preference):
1. Use git to clone this repository
2. From GitHub, you can use the `download` option to download this repository as a zip file (follow all instructions below, replacing the `git clone` step with download and unzip the zip file with the repository contents.
3. You can run the notebooks online with binder through: https://mybinder.org/v2/gh/simpeg/transform-2021-simpeg/master

To clone this repository, open up a terminal and navigate to where you want this repository stored on your computer.

Then run
```
git clone https://github.com/simpeg/transform-2021-simpeg.git
```
to clone the repository, and `cd` into the `transform-2021-simpeg` directory
```
cd transform-2021-simpeg
```

### Step 3: Create the AEM plot tutorial conda environment

From inside of the `aem_plot` repository, create the `aem_plot` conda environment
```
conda env create -f environment.yml
```
and activate the environment
```
conda activate aem_plot
```

### Step 4: Launching the notebooks

Once you have activated the conda environment, you can launch the notebooks
```
jupyter notebook
```
Jupyter will then launch in your web-browser.

If you are able to open any one of the notebooks and run the first cell, then you should be good to go!
If you run into issues, please post in the #t21-tue-simpeg slack channel.

## License

All code and text in this repository is free software: you can redistribute it and/or
modify it under the terms of the MIT License.
A copy of this license is provided in [LICENSE](LICENSE).

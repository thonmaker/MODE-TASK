<img src="https://img.shields.io/badge/python-2.7%2C%203.6-blue.svg" align="right"><img src="https://api.travis-ci.org/RUBi-ZA/MODE-TASK.svg?branch=master" align="right"><img src="https://readthedocs.org/projects/pymode-task/badge/?version=latest" align="right"> <img src='https://anaconda.org/nizamibilal1064/mode-task/badges/version.svg' align="right"> <img src='https://anaconda.org/nizamibilal1064/mode-task/badges/downloads.svg' align="right">

# MODE-TASK

Collection of tools for analysing normal modes and performing principal component analysis

pyMODE-TASK - a PyMol plugin for MODE-TASK is [available here](https://github.com/RUBi-ZA/pyMODE-TASK).

## Installation

*Download the project:*
```bash
git clone https://github.com/RUBi-ZA/MODE-TASK.git
cd MODE-TASK
```

*C++ scripts can be called from within a python environment using their corresponding ANM.py and getEigenVectors.py scripts. If the binaries do not exist the Python wrapper will attempt to complile them. To compile the C++ yourself, use the following commands:*
```
sudo apt install g++
g++ -I cpp/src/ ANM.cpp -o ANM

```

MODE-TASK can be used with a variety of Python enviroments and package managers, below are some of the options:

*Virtual environment using Python 2 and pip:*
```bash
sudo apt install virtualenvwrapper python-dev python-pip
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```
*Virtual environment using Python 3 and pip3:*
```bash
sudo apt install virtualenvwrapper python3-dev python3-pip
virtualenv venv
source venv/bin/activate
pip3 install setuptools
pip3 install -r requirements.txt
```
*Conda (Python version depends on Conda installation):*
```bash
conda create -n mode_task
source activate mode_task
conda install -c conda-forge numpy
conda install -c conda-forge cython
conda install -c omnia mdtraj
conda install -c conda-forge scipy
conda install -c conda-forge pandas
conda install -c conda-forge sklearn-contrib-lightning
conda install -c conda-forge matplotlib
```
Now <img src='https://anaconda.org/nizamibilal1064/mode-task/badges/installer/conda.svg'>:

```bash
conda install -c nizamibilal1064 mode-task
```
It will install the mode-task in /home/user/miniconda2/pkgs

## Usage

For more detailed documentation on installation and usage of the tool suite please see our [ReadTheDocs](http://mode-task.readthedocs.io/en/latest/index.html) site.

## Contributing to the project

Questions and issues can be posted to the [issue tracker](https://github.com/RUBi-ZA/MODE-TASK/issues).

Pull requests are welcome and will be reviewed however a guarentee can not me made as to your request being accepted.

To contribute to the documentation see [here](https://github.com/RUBi-ZA/MODE-TASK/tree/master/docs). The documentation is hosted by [ReadTheDocs](https://readthedocs.org/) and makes use of reStructuredText for markdown with Latex for mathematical equasions. See [here](https://docs.readthedocs.io/en/latest/getting_started.html) for a more detailed guideline on creating documentation for ReadTheDocs.

## Citation

**MODE-TASK: Large-scale protein motion tools**

*Caroline Ross, Bilal Nizami, Michael Glenister, Olivier Sheik Amamuddy, Ali Rana Atilgan, Canan Atilgan, Özlem Tastan Bishop;*

[Bioinformatics, Volume 34, Issue 21, 1 November 2018](https://academic.oup.com/bioinformatics/article/34/21/3759/5021681) <br/>
[![doi](http://img.shields.io/badge/doi-10.1093%2Fbioinformatics%2Fbty427-blue.svg?style=flat)](https://academic.oup.com/bioinformatics/article/34/21/3759/5021681) 
[![pubmed](http://img.shields.io/badge/pubmed-29850770-blue.svg?style=flat)](https://www.ncbi.nlm.nih.gov/pubmed/29850770)

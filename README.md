# Community-detection-Facebook-network

## Main objective

Develop a tool capable of identifying communities and influencers in a social network (Facebook).

## Context

This project is developed in Python 3 for the Social Media Analytics course (given by Prof. Dr. Philippe Cudré-Mauroux and Prof. Dr. Mourad Khayati) of the Master in Computer Science in the university of Fribourg, Switzerland.

This course is worth 5 ECTS points.

Spring 2020.

**Project supervisor**: Prof. Dr. Mourad Khayati

## Team members

- [Chacun Guillaume](https://github.com/ChacunGu)
- [Vorpe Fabien](https://github.com/fabienvorpe)

## Installation

This project has been developed and tested in a Jupyter Notebook with Python 3.8.1 64 bits on Windows 10 Professional.  There is no guarantee it will be working on any other configuration.

Multiple Python modules were used in this project. They were installed with Python's package manager pip. They are all listed along with their version in the file requirements.txt.

To simplify the installation process, please consider using a virtual environment.

### Required files

A directory named 'data' has to be created in the root directory. It must contain the Facebook dataset (file named 'facebook_combined.txt') - download link: http://snap.stanford.edu/data/egonets-Facebook.html, consulted the 25th March 2020)

### Virtual environment

Description of the installation and use of a Python's virtual environment on Windows.

Install the virtual environment module 'virtualenv':
```
pip install virtualenv
```

In the root directory of the project, create a new virtual environment:
```
<path to python.exe (3.8.1 64bits)> -m venv <environment's name>
```

Activate the virtual environment:
```
<environment's name>\Scripts\activate
```

You can then automatically install all the Python's modules required for the project to work:
```
pip install --upgrade -r requirements.txt
```

For more information about virtualenv please check the documentation on : https://python-guide-pt-br.readthedocs.io/fr/latest/dev/virtualenvs.html

## Usage

From the activated virtual environment, you can access the Jupyter Notebook:
```
jupyter notebook
```

You can then open the 'main.ipynb' file which contains the whole implementation. No modification must be made for the code to work. You can simply run all cells in order to obtain all the results of this project. Be aware that depending on the graph you use, the computing of the network's properties and the communities detection with Louvain can take several minutes (11 minutes for Louvain on the Facebook network).

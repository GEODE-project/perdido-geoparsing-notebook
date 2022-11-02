# Geoparsing Tutorial Notebook

Jupyter notebook for geoparsing historical encyclopedia texts in French using the [PERDIDO Geoparser](https://github.com/ludovicmoncla/perdido). 

This notebook is proposed by [L. Moncla](https://ludovicmoncla.github.io/) (INSA Lyon) and [K. McDonough](https://www.turing.ac.uk/people/researchers/katherine-mcdonough) (The Alan Turing Institute) as part of the [GEODE](https://geode-project.github.io/) project.

## Overview

In this tutorial, we demonstrate how to use a custom version of the [Perdido](https://github.com/ludovicmoncla/perdido) geoparser python library developed in the [GEODE](https://geode-project.github.io) project.
We will use texts from Diderot and d’Alembert’s *Encyclopédie* as a case study for querying a corpus and wrangling geoparsed data. We will also compare Perdido’s NER annotations (e.g. it's output) to the results of other well-known python NER libraries ([spaCy](https://spacy.io) and [Stanza](https://stanfordnlp.github.io/stanza/index.html)).



In this tutorial, we'll learn about a few different things.

- How to load data from TEI-XML files into a Python dataframe
- Use Python dataframe for simple data analysis
- Test the [PERDIDO API](http://erig.univ-pau.fr/PERDIDO/api.jsp) for preprocessing French texts (part-of-speech tagging)
- Test the [PERDIDO API](http://erig.univ-pau.fr/PERDIDO/api.jsp) for geoparsing (geotagging + geocoding) Encyclopedie articles
- Display custom geotagging results (PERDIDO TEI-XML) with the [displaCy Named Entity Visualizer](https://spacy.io/usage/visualizers)
- Display geocoding results on a map

## Open the notebook in the cloud

You can open this notebook in an executable and remote environment with [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GEODE-project/perdido-geoparsing-notebook/master?filepath=Tutorial-geoparsing.ipynb) or [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/GEODE-project/perdido-geoparsing-notebook/master/Tutorial-geoparsing.ipynb)



## Set up a python environment


### Clone this github repository

```bash
git clone https://github.com/GEODE-project/perdido-geoparsing-notebook.git
```


### Configure the environment with all dependencies

#### Method 1


* MacOS/Linux users: Create a new python environment called `tutorial-geoparsing-py39` with all dependencies using the `environment-osx-linux.yml` configuration file:

```bash
conda env create -f environment-osx-linux.yml
```

* Windows users: Create a new python environment called `tutorial-geoparsing-py39` with all dependencies using the `environment-win64.yml` configuration file:

```bash
conda env create -f environment-win64.yml
```

* Activate the environment

```bash
conda activate tutorial-geoparsing-py39
```

#### Method 2

* Create a new environment called `tutorial-geoparsing-py39`

```bash
conda create -n tutorial-geoparsing-py39 python=3.9
```

* Activate the environment

```bash
conda activate tutorial-geoparsing-py39
```

* Install dependencies with `pip`

```bash
pip install -r requirements.txt
```


### Launch the jupyter server

```bash
jupyter notebook
```



## Acknowledgement

Data courtesy the [ARTFL Encyclopédie Project](https://artfl-project.uchicago.edu/), University of Chicago.

The authors are grateful to the [ASLAN project](https://aslan.universite-lyon.fr/) (ANR-10-LABX-0081) of the Université de Lyon, for its financial support within the French program "Investments for the Future" operated by the National Research Agency (ANR).

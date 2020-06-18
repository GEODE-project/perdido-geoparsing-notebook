# Perdido Geoparsing Notebook
Jupyter notebook for geoparsing French historical documents with the PERDIDO Geoparser. 

You can open this notebook in an executable environment with [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ludovicmoncla/perdido-geoparsing-notebook/master?filepath=Geoparsing.ipynb)


This notebook is proposed by [L. Moncla](https://ludovicmoncla.github.io/) and [K. McDonough](http://kmcdono.com/) as part of the [GéoDISCO project](https://www.msh-lse.fr/projets/geodisco/).


## Overview

In this tutorial, we'll learn about a few different things.

- How to load data from TEI-XML files into a Python dataframe
- Use Python dataframe for simple data analysis
- Test the [PERDIDO API](http://erig.univ-pau.fr/PERDIDO/api.jsp) for preprocessing French texts (part-of-speech tagging)
- Test the [PERDIDO API](http://erig.univ-pau.fr/PERDIDO/api.jsp) for geoparsing (geotagging + geocoding) Encyclopedie articles
- Display custom geotagging results (PERDIDO TEI-XML) with the [displaCy Named Entity Visualizer](https://spacy.io/usage/visualizers)
- Display geocoding results on a map

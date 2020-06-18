# Perdido Geoparsing Notebook
Jupyter notebook for geoparsing French historical documents with the PERDIDO Geoparser. 

This notebook is proposed by [L. Moncla](https://ludovicmoncla.github.io/) and [K. McDonough](http://kmcdono.com/) as part of the [GéoDISCO](https://www.msh-lse.fr/projets/geodisco/) and GEODE projects.

## Overview

In this tutorial, we'll learn about a few different things.

- How to load data from TEI-XML files into a Python dataframe
- Use Python dataframe for simple data analysis
- Test the [PERDIDO API](http://erig.univ-pau.fr/PERDIDO/api.jsp) for preprocessing French texts (part-of-speech tagging)
- Test the [PERDIDO API](http://erig.univ-pau.fr/PERDIDO/api.jsp) for geoparsing (geotagging + geocoding) Encyclopedie articles
- Display custom geotagging results (PERDIDO TEI-XML) with the [displaCy Named Entity Visualizer](https://spacy.io/usage/visualizers)
- Display geocoding results on a map

## Open the notebook

You can open this notebook in an executable environment with [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GEODE-project/perdido-geoparsing-notebook/master?filepath=GeoparsingEncyclopedie.ipynb)

## Acknowledgement

Data courtesy the [ARTFL Encyclopédie Project](https://artfl-project.uchicago.edu/), University of Chicago.

This work was supported by the [ASLAN project](https://aslan.universite-lyon.fr/) (ANR-10-LABX-0081) of Université de Lyon, within the program « Investissements d’Avenir » (ANR-11-IDEX-0007) operated by the French National Research Agency (ANR).

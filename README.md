# CWI vs SAAR - Polynomial Interpolation
## Overview

This repository contains Python script in Jupiter Notebook and data files used in an analysis of Catchment Wetness Index (CWI) and Standard Average Annual Rainfall (SAAR) data, based on the NERC (1975) Flood Studies Report (FSR) - Fixed percentage runoff model Figure I.6.62.

The main goal of this project was to create a model that can predict the CWI value from a given SAAR value. To achieve this, we used polynomial fitting to find best fits a given set of data points.

Here's the chart in quetsion:

![image](https://github.com/Patryk-Obermajer/CWI-vs-SAAR---Polynomial-Interpolation/assets/69651910/a1881cb3-2cfa-4051-a235-b8089e834dbb)

Of course, for the majority of applications—particularly considering the resolution of the figure from which we extracted the data—this polynomial interpolation technique might be excessive. A simpler and potentially more efficient approach could be to employ linear interpolation between data points from the FSR dataset.

## Contents

Inside this repository, you'll find:

- Python scripts in a Jupiter Notebook.
- The `SAAR_CWI.csv` file containing our dataset extracted from the FSR.
- Images of the graph we were aiming to reproduce and the graph resulting from our model.

## Results

We found that a 16-degree polynomial model fits our data. We achieved a very reliable R-squared score of 0.9999 and a low RMSE of 0.1926, indicating a high level of prediction accuracy.
Moreover, our model exhibited consistent performance across the entire SAAR value range.


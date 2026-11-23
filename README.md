# eROSITA Cluster Scaling Relations

Code and analysis files for the PHYS 474 – Galaxies final project.

This project investigates the scaling relations between galaxy cluster temperature, mass, and luminosity using the eROSITA eRASS1 cluster catalogue from Bulbul et al. (2024). The observed relations are compared with the self-similar predictions for the mass–temperature (M–T) and luminosity–temperature (L–T) relations.

`phys474_finalproject.ipynb` contains the main analysis, including data selection and cleaning, linear regression fits, uncertainty calculations, and comparisons across different temperature ranges.

The analysis considers three fitting approaches: unweighted linear regression, weighted regression accounting for uncertainties in the dependent variable, and a weighted method that accounts for uncertainties in both variables.

The eRASS1 cluster catalogue is available through the [eROSITA DR1 data release](https://erosita.mpe.mpg.de/dr1/). However, the catalogue is not included in this repository and can be obtained separately.

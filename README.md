# eROSITA Cluster Scaling Relations

This project investigates galaxy cluster mass–temperature (M–T) and luminosity–temperature (L–T) scaling relations using the eROSITA eRASS1 cluster catalogue.

The observed relations are compared with the self-similar predictions:

- **M–T:** `M ∝ T^(3/2)`
- **L–T:** `L ∝ T^2`

## Data

The analysis uses the eRASS1 catalogue from Bulbul et al. (2024), including temperature (`KT`), mass (`M500`), and luminosity (`Lbol500`). The catalogue is available through the [eROSITA DR1 data release](https://erosita.mpe.mpg.de/dr1/).

## Methods

The notebook includes data cleaning and fitting using unweighted, weighted, and iterative methods that account for measurement uncertainties. Fits are also repeated across different temperature ranges.

## Running the Code

`phys474_finalproject.ipynb` contains the main analysis. Update the catalogue file path before running the notebook.

## Reference

Bulbul, E., et al. (2024), *The SRG/eROSITA All-Sky Survey: The first catalog of galaxy clusters and groups in the western Galactic hemisphere*.

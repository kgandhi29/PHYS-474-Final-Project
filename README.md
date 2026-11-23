# PHYS-474-Final-Project

## eROSITA Cluster Scaling Relations

This project investigates the scaling relations between galaxy cluster temperature, mass, and luminosity using the eROSITA eRASS1 cluster catalogue.

The analysis focuses on comparing the observed relations with the self-similar predictions:

- Mass–Temperature (M–T): \(M \propto T^{3/2}\)
- Luminosity–Temperature (L–T): \(L \propto T^2\)

### Data

The analysis uses the eRASS1 cluster catalogue from Bulbul et al. (2024). The relevant quantities are:

- `BEST_Z`: Best redshift estimate
- `KT`: Cluster temperature
- `M500`: Cluster mass
- `Lbol500`: Bolometric luminosity

The catalogue is not included in this repository. The data must be obtained separately at https://erosita.mpe.mpg.de/dr1/AllSkySurveyData_dr1/Catalogues_dr1/ from the eROSITA/eRASS1 galaxy groups and clusters primary catalogue.

### Methods

The code:

1. Selects clusters with valid, positive measurements.
2. Converts temperature, mass, and luminosity to logarithmic values.
3. Fits the M–T and L–T scaling relations using:
   - Unweighted linear regression
   - Weighted regression using uncertainties in the dependent variable
   - Weighted regression accounting for uncertainties in both variables
4. Divides the sample into temperature bins and repeats the fits.
5. Compares the resulting slopes with the self-similar predictions.

### Requirements

The analysis uses Python and the following packages:

- NumPy
- Pandas
- Matplotlib
- Astropy

### Running the Code

After obtaining the eRASS1 catalogue, update the file path in the notebook or script to point to the local catalogue file. Then run the analysis.

### Main Reference Paper

Bulbul, E., et al. (2024), *The SRG/eROSITA All-Sky Survey: The first catalog of galaxy clusters and groups in the western Galactic hemisphere*.

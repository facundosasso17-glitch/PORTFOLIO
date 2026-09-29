# Raw data

Place the two source CSV files used by the original analysis in this folder:

1. `EAH_2023_ind.csv`
2. `Precio alquiler_Ba_ciudad_csv.csv`

The notebook expects these exact filenames.

## Why are the datasets not committed to GitHub?

The portfolio repository should contain the code and documentation, not large raw microdata files. Keep the repository lightweight and link to the official public data sources instead.

## Geographic data

The commune GeoJSON is loaded directly from the Buenos Aires City open-data infrastructure by the notebook.

Official commune dataset:
https://data.buenosaires.gob.ar/dataset/comunas

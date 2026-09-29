# Rental Prices and Income Inequality in Buenos Aires City

## Portfolio project

**Question:** Do rental prices follow the spatial distribution of income across Buenos Aires City's communes?

This project explores the relationship between average family per-capita income and average rental prices across the 15 communes of Buenos Aires City.

### Key result from the original analysis

The original exploratory run found a **Pearson correlation of 0.87** between average family per-capita income and average rental prices across the 14 communes for which rental data were available.

This result should be interpreted cautiously because the datasets are **not contemporaneous**:

- Income: EAH 2023
- Rental prices: 2018–2019

Therefore, this project examines **spatial association**, not current housing affordability.

## Data

### EAH 2023

Individual-level data from the Buenos Aires City Household Survey (EAH), using:

- commune
- family per-capita income
- sex

Only positive income observations are retained.

### Rental prices

Historical rental-price data by commune from Buenos Aires City, filtered to 2018 and 2019 and averaged across those two years.

### Geographic data

Official Buenos Aires City commune boundaries.

Source:
https://data.buenosaires.gob.ar/dataset/comunas

## Repository structure

```text
PORTFOLIO/
└── rental-income-caba/
    ├── rental_income_caba.ipynb
    ├── README.md
    ├── requirements.txt
    ├── .gitignore
    └── data/
        └── raw/
            └── README.md
```

Raw datasets are intentionally not included in this repository. See `data/raw/README.md`.

## Methods

- Data cleaning
- Exploratory data analysis
- Descriptive statistics
- Grouping and aggregation by commune
- Pearson correlation
- Linear descriptive residuals
- Spatial data integration
- Choropleth mapping

## Main findings

1. Income and rental prices show a strong positive spatial association in the observed data.
2. Commune 14 has the highest average income in the EAH 2023 data used here.
3. Commune 14 also has the highest average rental price in the 2018–2019 rental dataset.
4. Commune 8 has income data but no rental-price observation in the selected historical period.
5. High within-commune dispersion shows why commune-level averages should not be interpreted as homogeneous social spaces.
6. Commune 1 is especially relevant for further research because its aggregate indicators combine highly heterogeneous urban areas.

## Important methodological decision

The original notebook had a geographic merge problem caused by joining commune geometry to the analytical dataframe index. The portfolio version explicitly merges on the `comuna` variable:

```python
geo_analysis = communes_geo.merge(
    analysis,
    on="comuna",
    how="left",
    validate="one_to_one"
)
```

This keeps commune identifiers aligned and makes missing rental data visible on the map.

## Limitations

The temporal mismatch between income and rental data is the central limitation. The analysis should not be interpreted as a contemporaneous rent-burden or affordability estimate.

A future version should use rental and income data from the same period and, ideally, analyze neighborhoods and housing typologies.

## Tools

**Python · Pandas · NumPy · Matplotlib · Seaborn · GeoPandas · SciPy**

**Research:** social research · housing research · exploratory data analysis · spatial analysis · survey data · data visualization

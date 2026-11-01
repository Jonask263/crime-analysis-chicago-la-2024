# Comparative Crime Analysis: Chicago vs. Los Angeles (2024)

A Python-based comparison of crime patterns in Chicago and Los Angeles in 2024, with a focus on **violent crime**, **property crime**, **time of day** and **location types**.

## Research question

How do time-of-day and location patterns differ between violent and property crimes in Chicago and Los Angeles?

## Project workflow

1. **Data cleaning:** Inspect missing values and prepare the relevant attributes in each dataset.
2. **Data harmonization:** Align crime categories and other fields to make the two cities comparable.
3. **Exploratory analysis:** Explore and visualize patterns by crime category, time and location.
4. **Association rule mining:** Apply the Apriori algorithm and association rules to examine recurring time–location combinations.
5. **Comparison:** Compare findings across crime categories and the two cities.

## Technologies

- Python
- pandas
- Matplotlib
- mlxtend (Apriori and association rules)
- Jupyter Notebook

## Main findings

The notebook reports associations between time of day and location, with lift values above 1 for certain combinations. In this analysis, **property crime** was associated particularly with **evening/public** combinations, while **violent crime** showed an association with **night/residential** combinations. The strengths of some associations differed between Chicago and Los Angeles.

These are descriptive associations based on the selected datasets and category definitions; they do **not** establish causation.

## Data and reproducibility

The original CSV datasets are **not included** in this repository. The notebook expects the following files in the same directory as `CrimeAnalysis.ipynb`:

- `lapd_nibrs.csv` – Los Angeles dataset (read with `sep=";"`)
- `ccd.csv` – Chicago dataset (read with `sep=","`)

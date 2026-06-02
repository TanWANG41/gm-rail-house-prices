# Rail Accessibility and House Prices in Greater Manchester

This repository contains a spatial urban analytics project examining the relationship between rail accessibility and residential house prices in Greater Manchester.

The project uses residential transaction data from 2023 to 2025 and combines it with postcode locations, neighbourhood deprivation, city-centre distance, LSOA boundaries, and rail/Metrolink station locations.

## Workflow

1. **Data collection and integration**
   Residential transaction records were combined with postcode geography, deprivation data, administrative boundaries, and rail/Metrolink station locations.

2. **Data cleaning and preparation**
   The dataset was filtered to Greater Manchester, cleaned for missing or unsuitable records, and transformed into a spatial dataset suitable for analysis.

3. **Feature engineering**
   Key variables were created, including distance to the nearest station, distance to Manchester city centre, deprivation measures, log-transformed house prices, and categorical property controls.

4. **Exploratory spatial analysis**
   Summary statistics, price distributions, and spatial maps were used to understand the structure of the data before modelling.

5. **Regression analysis**
   An OLS model was used to estimate the average relationship between station distance and house prices. Spatial diagnostics were then used to assess whether this relationship varied geographically.

6. **GWR analysis**
   A Geographically Weighted Regression model was used to explore local variation in the station-distance relationship across Greater Manchester.

## Repository files

* `3149531_URBAN5160.ipynb` — main Jupyter Notebook with code, outputs, maps, models, and written report
* `README.md` — project overview

## Main result

The analysis suggests that distance to the nearest rail or Metrolink station is associated with residential transaction prices in Greater Manchester. However, the GWR results show that this relationship is not spatially uniform across the city-region.

The findings should be interpreted as associations rather than causal effects.


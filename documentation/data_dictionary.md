# Data Dictionary

This document describes the variables present in the dataset.

| Column | Type | Description | Unit | Source | Notes |
|------|------|-------------|------|-------|------|
| id | Integer | Unique identifier for each record | – | Author | Sequential index |
| state | Categorical | Name of the Brazilian state | – | IBGE | Official state names |
| state_code | Categorical | Two-letter abbreviation of the state | – | IBGE | Example: SP, RJ |
| region | Categorical | Geographic macro-region | – | IBGE | North, Northeast, Central-West, Southeast, South |
| region_code | Integer | Numeric region identifier | – | Author | Used for computational analysis |
| year | Integer | Reference year of the dataset | year | Author | Current dataset uses 2023 |
| pm25_mean | Numeric | Annual mean PM2.5 concentration | µg/m³ | IQAir / OpenAQ | Capital city used as proxy |
| pm25_category | Ordinal | Air quality category derived from PM2.5 | – | Derived variable | Based on defined thresholds |
| sanitation_coverage_pct | Numeric | Population with sanitation services | % | SNIS | Brazilian sanitation database |
| wildfire_hotspots_thousands | Numeric | Number of wildfire hotspots | thousands | INPE | Satellite monitoring |
| respiratory_hospitalizations_per100k | Numeric | Respiratory hospitalizations | per 100k inhabitants | DATASUS | Health information system |
| life_expectancy | Numeric | Life expectancy at birth | years | IBGE | Demographic statistics |
| primary_care_coverage_pct | Numeric | Primary health care coverage | % | e-Gestor APS | Brazilian health system |

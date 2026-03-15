# Data Dictionary

This document describes the variables present in the dataset.

| Column                       | Type        | Description                                                       | Unit            | Source                                   | Notes                            |
| ---------------------------- | ----------- | ----------------------------------------------------------------- | --------------- | ---------------------------------------- | -------------------------------- |
| id                           | integer     | Unique identifier for each observation                            | —               | generated                                | state–year combination           |
| year                         | integer     | Year of observation                                               | year            | IBGE                                     | temporal dimension               |
| state                        | categorical | Brazilian federative unit name                                    | —               | IBGE                                     |                                  |
| state_code                   | categorical | Two-letter state abbreviation                                     | —               | IBGE                                     |                                  |
| region                       | categorical | Geographic region (North, Northeast, Midwest, Southeast, South)   | —               | IBGE                                     |                                  |
| pm25_mean                    | numeric     | Annual mean concentration of fine particulate matter (PM2.5)      | µg/m³           | OpenAQ / Copernicus                      | indicator of air pollution       |
| pm10_mean                    | numeric     | Annual mean concentration of particulate matter PM10              | µg/m³           | OpenAQ / Copernicus                      |                                  |
| no2_mean                     | numeric     | Annual mean nitrogen dioxide concentration                        | µg/m³           | OpenAQ                                   | traffic-related pollutant        |
| o3_mean                      | numeric     | Annual mean ozone concentration                                   | µg/m³           | Copernicus Atmosphere Monitoring Service | secondary pollutant              |
| wildfire_hotspots            | numeric     | Annual number of detected wildfire hotspots                       | count           | INPE Queimadas                           | proxy for biomass burning        |
| deforestation_rate           | numeric     | Annual deforested area                                            | km²             | INPE PRODES                              | environmental pressure indicator |
| respiratory_hospitalizations | numeric     | Hospitalizations due to respiratory diseases per 100k inhabitants | cases/100k      | DATASUS                                  | ICD-10 respiratory codes         |
| asthma_rate                  | numeric     | Hospitalization rate for asthma                                   | cases/100k      | DATASUS                                  | respiratory disease indicator    |
| copd_rate                    | numeric     | Hospitalization rate for chronic obstructive pulmonary disease    | cases/100k      | DATASUS                                  | COPD indicator                   |
| respiratory_mortality        | numeric     | Mortality rate due to respiratory diseases                        | deaths/100k     | DATASUS                                  | health outcome indicator         |
| sanitation_coverage          | numeric     | Population with access to sanitation services                     | %               | SNIS / IBGE                              | environmental health factor      |
| primary_care_coverage        | numeric     | Coverage of primary healthcare services                           | %               | Ministry of Health                       | health infrastructure            |
| hospital_beds_per1000        | numeric     | Number of hospital beds per 1000 inhabitants                      | beds/1000       | Ministry of Health                       | healthcare capacity              |
| population_density           | numeric     | Population density                                                | inhabitants/km² | IBGE                                     | demographic exposure factor      |
| gdp_per_capita               | numeric     | Gross domestic product per capita                                 | BRL             | IBGE                                     | socioeconomic indicator          |
| annual_mean_temperature      | numeric     | Mean annual air temperature                                       | °C              | INMET                                    | climate condition                |
| relative_humidity            | numeric     | Mean annual relative humidity                                     | %               | INMET                                    | affects pollutant dispersion     |
| urbanization_rate            | numeric     | Percentage of population living in urban areas                    | %               | IBGE                                     | urban exposure indicator         |


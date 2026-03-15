# Data Dictionary

This document describes the variables present in the dataset.

Column;Type;Description;Unit;Source;Notes
id;integer;Unique identifier for each observation;—;generated;State-year combination
year;integer;Year of observation;year;IBGE / study design;Temporal dimension
state;categorical;Brazilian federative unit name;—;IBGE;State name
state_code;categorical;Two-letter state abbreviation;—;IBGE;UF code
region;categorical;Geographic region;—;IBGE;North, Northeast, Midwest, Southeast, South
pm25_mean;numeric;Annual mean concentration of fine particulate matter (PM2.5);µg/m³;OpenAQ / Copernicus (target source for real data);Air pollution indicator
pm10_mean;numeric;Annual mean concentration of particulate matter PM10;µg/m³;OpenAQ / Copernicus (target source for real data);Air pollution indicator
no2_mean;numeric;Annual mean nitrogen dioxide concentration;µg/m³;OpenAQ (target source for real data);Traffic-related pollutant
o3_mean;numeric;Annual mean ozone concentration;µg/m³;Copernicus (target source for real data);Secondary pollutant
wildfire_hotspots;numeric;Annual number of detected wildfire hotspots;count;INPE Queimadas (target source for real data);Proxy for biomass burning
deforestation_rate;numeric;Annual deforested area;km²;INPE PRODES (target source for real data);Environmental pressure indicator
respiratory_hospitalizations;numeric;Hospitalizations due to respiratory diseases per 100k inhabitants;cases/100k;DATASUS (target source for real data);Respiratory health outcome
asthma_rate;numeric;Hospitalization rate for asthma;cases/100k;DATASUS (target source for real data);Asthma burden indicator
copd_rate;numeric;Hospitalization rate for chronic obstructive pulmonary disease;cases/100k;DATASUS (target source for real data);COPD burden indicator
respiratory_mortality;numeric;Mortality rate due to respiratory diseases;deaths/100k;DATASUS (target source for real data);Respiratory mortality outcome
sanitation_coverage;numeric;Population with access to sanitation services;%;SNIS / IBGE (target source for real data);Environmental health infrastructure
primary_care_coverage;numeric;Coverage of primary healthcare services;%;Ministry of Health (target source for real data);Primary healthcare infrastructure
hospital_beds_per1000;numeric;Number of hospital beds per 1000 inhabitants;beds/1000;Ministry of Health (target source for real data);Healthcare capacity
population_density;numeric;Population density;inhabitants/km²;IBGE (target source for real data);Demographic exposure factor
gdp_per_capita;numeric;Gross domestic product per capita;BRL;IBGE (target source for real data);Socioeconomic indicator
annual_mean_temperature;numeric;Mean annual air temperature;°C;INMET (target source for real data);Climate condition
relative_humidity;numeric;Mean annual relative humidity;%;INMET (target source for real data);Affects pollutant dispersion
urbanization_rate;numeric;Percentage of population living in urban areas;%;IBGE (target source for real data);Urban exposure indicator
pm25_category;categorical;PM2.5 annual air-quality class;category;Applied rule (WHO-inspired thresholds);Derived from pm25_mean
pm10_category;categorical;PM10 annual air-quality class;category;Applied rule (threshold bins);Derived from pm10_mean
no2_pollution_level;categorical;NO2 annual pollution level;category;Applied rule (threshold bins);Derived from no2_mean
o3_pollution_level;categorical;O3 annual pollution level;category;Applied rule (threshold bins);Derived from o3_mean
wildfire_intensity;categorical;Wildfire activity level;quartile class;Applied rule (sample quartiles);Derived from wildfire_hotspots
deforestation_level;categorical;Deforestation pressure level;quartile class;Applied rule (sample quartiles);Derived from deforestation_rate
respiratory_risk_level;categorical;Overall respiratory hospitalization burden level;quartile class;Applied rule (sample quartiles);Derived from respiratory_hospitalizations
asthma_risk_level;categorical;Asthma burden level;quartile class;Applied rule (sample quartiles);Derived from asthma_rate
copd_risk_level;categorical;COPD burden level;quartile class;Applied rule (sample quartiles);Derived from copd_rate
respiratory_mortality_level;categorical;Respiratory mortality burden level;quartile class;Applied rule (sample quartiles);Derived from respiratory_mortality
sanitation_level;categorical;Sanitation coverage class;category;Applied rule (infrastructure thresholds);Derived from sanitation_coverage
primary_care_level;categorical;Primary care coverage class;category;Applied rule (coverage thresholds);Derived from primary_care_coverage
hospital_bed_capacity;categorical;Hospital bed availability class;category;Applied rule (capacity thresholds);Derived from hospital_beds_per1000
population_density_class;categorical;Population density class;category;Applied rule (urbanity thresholds);Derived from population_density
economic_level;categorical;GDP per capita class;category;Applied rule (income-like thresholds);Derived from gdp_per_capita
temperature_zone;categorical;Annual temperature zone;category;Applied rule (climate thresholds);Derived from annual_mean_temperature
humidity_level;categorical;Annual humidity level;category;Applied rule (climate thresholds);Derived from relative_humidity
urbanization_class;categorical;Urbanization class;category;Applied rule (urbanization thresholds);Derived from urbanization_rate


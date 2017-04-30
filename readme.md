# ADL DataDive Repo
This repository was created while working on a DataKind datadive for ADL.

Currently, this is mostly data cleaning and munging. There are some interesting datasets in the output folder.

- `incidents_supplemented_2.csv` combines the state level aggregated hate crime data with census population estimates, enhanced penalty law information, other statute information, and creates per capita measurements of hate crime types
	- the `race_corrected` column is the `race_ethnicity_ancestry` column for 2015, and for prior years it is the `race` and `ethnicity` columns added together. The definitions changed in 2015. Hopefully this is a fair comparison
- `table_12_2004-2015.csv` is the yearly agency reporting data (aka "table 12") from the FBI UCR Hate Crime Statistics. https://ucr.fbi.gov/hate-crime
- `incident_aggregated_with_agencies.csv` is the supplemented incident data above merged with the table 12 agency data for the years 2004-2015.
	- There is a calculated field labled `percent_population_covered` which is the `population covered` field divided by the `est_pop` (estimated population) field



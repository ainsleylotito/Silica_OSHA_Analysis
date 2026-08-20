Respirable Silica Analysis
================

## Overview

This repository contains code and data for analyzing respirable silica
workplace exposures.

## Data

Raw datafiles are in the `/RawData` directory. -
Respirable_Silica_Data.txt contains the OSHA samples from 1984-2026 for
**Silica, Crystaline, and Mixed Respirable (Quartz, Cristobalite,
Tridymite)** \[IMIS Code: 9000\]. Data was restricted to industries
categorized as NAICS:327991. Data were pulled on August 20, 2026.

### Data sources:

- **OSHA Chemical Exposure Health Data**: The database contains
  industrial hygiene samples submitted to the OSHA Technical Center from
  1984 onward. Data can be queried on [this
  page](https://www.osha.gov/opengov/health-samples), and the data
  dictionary may be found
  [here](https://www.osha.gov/opengov/osha-health-samples-dataset-field-definitions).

## Methods

Data are cleaned in the `Scripts/Cleaning.rmd` file. Cleaned datasets
are in the `CleanData` Directory. A data dictionary is included in the
file `DataDictionary.xlsx`. Analyses were conducted in R using tidyverse
and \[packages\] tools.

## Reproducibility

All analyses can be reproduced by running the scripts in the `/Scripts`
directory, starting with `01_Cleaning` then `02_Analysis`.

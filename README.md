# R4 Marine Science

## About This Repository

This repository documents my work in **R for Marine Science**, focusing on reproducible data workflows, ecological data wrangling, visualisation, and the use of R to extract biological signals from complex environmental datasets.

The module builds progressively from foundational data manipulation and visualisation to advanced data rescue workflows, relational data management, and an independent ecological Keystone analysis.

---

## Workshop 1 — Foundations of Data Science: Wrangling and Plotting

Workshop 1 focused on establishing a reproducible R workflow and strengthening fundamental data science skills through an **AI-Off** approach.

### Key topics

- R project and workspace setup
- Git and GitHub repository configuration
- Reproducible folder architecture
- Workspace and environment management
- Importing CSV, TSV, and Excel data
- Understanding tibbles and data frames
- Data inspection with `glimpse()` and `summary()`
- Core `dplyr` grammar:
  - `select()`
  - `filter()`
  - `arrange()`
  - `mutate()`
  - `group_by()`
  - `summarise()`
- Pipe-based workflows
- Handling missing values
- Descriptive ecological summaries
- Introductory `ggplot2` layer logic
- Exporting figures and summary tables

### Dataset

The **Palmer Penguins** dataset was used to practise data wrangling and investigate morphological variation among penguin species and islands.



---

## Workshop 2 — Advanced Data Wrangling: Extracting Ecological Signals from Noisy Systems

Workshop 2 expanded the foundational skills from Workshop 1 by introducing more complex data structures and ecological data-cleaning challenges.

### Key topics

- Principles of tidy data
- Reshaping datasets with:
  - `pivot_longer()`
  - `pivot_wider()`
- Separating and combining variables
- String cleaning with `stringr`
- Date and time parsing with `lubridate`
- Relational data and joins:
  - `left_join()`
  - `inner_join()`
  - `anti_join()`
- Handling missing and erroneous values
- Converting legacy sensor errors to `NA`
- Distinguishing true absence from missing observations
- Explicit zero engineering using `complete()` and `coalesce()`
- Integrating biological and environmental datasets
- Transitioning from **AI-Off to AI-On**


---

## Keystone Exercise — Estuary Fish Survey: Data Rescue Mission

The Keystone exercise integrates the skills developed across both workshops into a single ecological data rescue workflow.

The project investigates relationships between **water quality and predatory fish assemblages along the Ross River Estuary gradient**.

### Data Sources

The analysis integrates four datasets:

1. Fish catch records
2. Site and spatial metadata
3. High-frequency water-quality sonde data
4. Species taxonomy dictionary

### Data Rescue Workflow

The Keystone workflow includes:

**Raw Data**

↓

**Data Ingestion**

↓

**String and Date Standardisation**

↓

**Sensor Error Cleaning**

↓

**Relational Joins**

↓

**Daily Environmental Summaries**

↓

**Taxonomic Translation**

↓

**Zero-Catch Framework**

↓

**Master Ecological Dataset**

↓

**Statistical Summaries**

↓

**Ecological Visualisation**


### Final Outputs

The Keystone analysis produces:

- A cleaned master ecological dataset
- Summary statistics for fish abundance and environmental conditions
- A multi-panel ecological figure showing species abundance along the salinity gradient

---

## Core R Packages

```r
library(tidyverse)
library(readxl)
library(stringr)
library(lubridate)
library(here)

## Author

**Agustinus Satrio Supoyo**  
Master of Marine Biology  
James Cook University

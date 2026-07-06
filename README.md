# Evaluating the 2022 Assistive Technology Act

An econometrics research pipeline built in R to evaluate the impact of the 2022 reauthorization of the 21st Century Assistive Technology Act on technology accessibility for disabled Americans.

## Overview

Although the 2022 reauthorization of the Assistive Technology Act increased federal funding for state assistive technology programs, little quantitative research has evaluated whether the policy improved technology access.

This project combines multiple public datasets into a unified panel dataset and applies econometric methods to evaluate whether increased funding translated into greater access to assistive technology.

The accompanying paper was completed through the UCSB Summer Research Academies (Policy Puzzle track).

---

## Research Question

> Has the 2022 Assistive Technology Act improved access to assistive technology and digital technology for Americans with disabilities?

---

## Data Sources

This project merges state-level panel data from several public datasets:

- **Administration for Community Living (ACL)** — state grant allocations (2016–2024)
- **Center for Assistive Technology Act Data Assistance (CATADA)** — assistive technology device loan data
- **Current Population Survey Computer & Internet Use Supplement (NTIA/Census)** — internet and device access among disabled individuals
- **American Community Survey (ACS)** — demographic controls

---

## Methods

The analysis includes:

- Data cleaning and preprocessing
- Automated dataset merging
- Exploratory data visualization
- Multiple linear regression
- Two-way fixed effects models
- Regression discontinuity analysis

The workflow was designed to automate repetitive data preparation so new specifications and robustness checks could be run with minimal manual work.

---

## Key Findings

- The 2022 reauthorization significantly increased state grant allocations.
- Higher grant funding was associated with increased assistive technology device loans.
- The policy did **not** produce statistically significant short-term improvements in internet or digital device access for disabled Americans.
- Results suggest that administrative implementation—not simply funding levels—may be limiting policy effectiveness.

---

## Repository Structure

```
data/              Raw public datasets
clean_data/        Processed datasets
figures/           Generated visualizations
scripts/           Data cleaning and econometric analysis
paper/             Final research paper
```

---

## Technologies

- R
- tidyverse
- fixest
- rdrobust
- ggplot2
- dplyr

---

## Future Work

Potential extensions include:

- Difference-in-differences estimation
- County-level analysis
- Longer post-policy observation window
- Additional demographic controls
- Interactive dashboard for policy exploration

---

## Authors

Chelsea Xie  
Henry Hussey  
Evelyn Oh

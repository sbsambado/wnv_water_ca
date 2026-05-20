# Water availability & WNV hotspots

This repository contains the full workflow for analyzing environmental and hydrological drivers of West Nile Virus (WNV) patterns in California. 

---

## Workflow Overview

1. **Data Download**
   - WNV surveillance & environmental covariates are downloaded & standardized.
   - Scripts: `scripts/01_download/`

2. **Data Cleaning**
   - Cleaning and harmonization of mosquito surveillance & environmental datasets.
   - Scripts: `scripts/02_clean/`

3. **Data Processing**
   - Construction of panel datasets & spatial clustering of clusterIDs.
   - Scripts: `scripts/03_process/`

4. **Statistical Analysis**
   - Panel regression models & summary analyses.
   - Scripts: `scripts/04_analysis/`

5. **Figure Generation**
   - Production of manuscript & supplementary figures.
   - Scripts: `scripts/05_figures/`
   - Outputs saved in `outputs/figures/`

6. **Sensitivity Analyses**
   - Robustness checks & alternative model specifications.
   - Scripts: `scripts/06_sensitivity/`

---


## Data Accessibility

Raw data are **not included in this repository**.

The `data/` directory is intentionally excluded via `.gitignore` to avoid uploading large or sensitive datasets.

---

## Reproducibility

This project uses [`renv`](https://rstudio.github.io/renv/) for dependency management.

To restore the environment:

```r
renv::restore()

# **Agricultural and Forestry Sampling Project**

## **Project Description**
This project is focused on developing a two-stage sampling plan for agricultural and forestry surveys, targeting key variables such as agricultural area, livestock populations, and forest resources. The methodology ensures precise and representative estimates at the provincial or strata levels, leveraging robust statistical techniques.

### **Objectives**
1. Design a representative two-stage sampling plan.
2. Apply stratification techniques based on multivariate criteria (`ag_area` and `TLUs_total`).
3. Select primary and secondary sampling units using probabilistic methods (PPS and SRSWOR).
4. Estimate totals, means, and coefficients of variation for key variables.
5. Provide a methodological framework adaptable to agricultural and forestry contexts.

---

## **Project Structure**
- **Data Sources**:
  - The dataset is derived from the **General Census of Population, Housing, Agriculture, and Livestock (RGPHAE)** module.
  - Key variables:
    - `province`: Province code.
    - `zone`: Geographical zone code.
    - `ag_area`: Total agricultural area (in hectares).
    - `TLUs_total`: Total Livestock Units (TLUs).
    - `ag_holdings`: Total number of agricultural holdings.

- **Codebase**:
  - R scripts for data cleaning, stratification, sample selection, and statistical analysis.

- **Key Steps**:
  1. Clean and prepare the data (`rgphae_ag_module`).
  2. Stratify primary sampling units (PSUs) using multivariate criteria.
  3. Select PSUs using the PPS method and secondary units (households) via SRSWOR.
  4. Estimate totals, means, and sampling errors.

---

## **Installation**
To run this project, ensure you have the following:
- **R** (version ≥ 4.0)
- Required R packages:
  ```r
  install.packages(c("dplyr", "tidyverse", "survey", "samplingbook"))

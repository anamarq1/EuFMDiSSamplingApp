# EuFMDiS sample size calculator
A Sampling App to Support the Calculation of Sampling Efforts during Foot- and-Mouth Disease Outbreaks

The EuFMDiS Sampling App aims to bring together the specific rules for sampling
outlined in the national sampling protocol for Denmark in the event of a FMD outbreak
with the simulation results from the EuFMDiS model. The app compliments the output of
the EuFMDiS model through a friendly interface to visualize and explore sample size
estimates in the event of an outbreak.


The app link is available at https://tipton-arpm.shinyapps.io/eufmdisSampling/


## Reproducibility, Software Environment & Demonstration Data

### Epidemiological Model
The demonstration simulation datasets processed by this application were generated using **EuFMDiS version 1.36**.

### R Dependencies & Software Versions
The web application was developed in **R** using the following key packages:

* **Framework & UI:** `shiny` (v1.8.0), `bslib` (v0.9.0), `shinydashboard` (v0.7.3), `shinyjs` (v2.1.0), `shinycssloaders` (v1.0.0)
* **Data Wrangling:** `data.table` (v1.15.0), `dplyr` (v1.1.4), `tidyr` (v1.3.1)
* **Visualization:** `ggplot2` (v3.5.1), `ggforce` (v0.4.2), `ggbreak` (v0.1.6)
* **Interactive Data Tables:** `DT` (v0.31)

### Demonstration Datasets
To support full open-science reproducibility and allow users to reproduce all metrics, tables, and visual outputs reported in the manuscript, raw simulation output files for both outbreak scenarios are provided directly in this repository:

1. **Scenario 1 (Fixed Index Herd):**
   * `denmark_fmd_demo_500runs_surveillance.csv`
   * `denmark_fmd_demo_500runs_summary.csv`
2. **Scenario 2 (Random Index Herds):**
   * `denmark_fmd_demo_500runsMay26random1_summary.csv` 
   * `denmark_fmd_demo_500runsMay26random1_surveillance.csv` 

Users can load these CSV files directly into the web application to reproduce the daily temporal distributions, holding summaries, and overall diagnostic test requirements (PCR and ELISA).


# Estimating the Effects of Fine Particulate Matter on 432 Cardiovascular Diseases Using Multi-Outcome Regression With Tree-Structured Shrinkage

# Author Contributions Checklist Form

## Data

### Abstract

Two raw dataset were used for our analysis. The first is daily average PM2.5 in micrograms per cubic meter from 2000 to 2012 inclusive for all zip codes in the mainland USA. The second is all hospitalizations among US Medicare beneficiaries aged 65+. The medicare dataset includes fields for date of hospitalization and the primary diagnosis on discharge, as denoted by codes from International Classification of Diseases, Revision 9 (ICD9).


### Availability 

The raw Medicare data cannot be made publicly available due to restrictions laid out in a Data Use Agreement (DUA) with the Centers for Medicare & Medicaid Services, US Department for Health and Human Services.

### Description 

Permissions: Medicare data were provided by the Centers for Medicare & Medicaid Services under the DUA mentioned above. More information can be provided upon request.

## Code

### Abstract

We provide code for: (1) fitting the spike and slab MOReTreeS model (ssMOreTreeS) via the variational inference algorithm described in our manuscript; (2) re-running the simulation study; (3) reproducing the results of the data example (although as data is not provided, this code cannot be run), and; (4) recreating all tables and figures in the manuscript (other than figures created using LaTeX code.

### Description

How delivered: R code available on GitHub
Licensing information (default is MIT License):
Link to code/repository: https://github.com/emgthomas/moretrees


## Instructions for Use

### Reproducibility 

All simulations can be re-run. The following tables and figures from the manuscript can be fully reproduced: Figure 3, Figures A.2 and A.6, Tables A.1 and A.2. All simulations can be reproduced. However, figures and tables related to the simulations can also be reproduced without re-running the simulations as full simulation results have been provided. 

Simulations and relevant tables/figures can be reproduced by running the R scripts simulations.R followed by simulations_figures_and_tables.R Simulation scenarios are denoted by the parameter simidx (which takes integer values 1 through 8) in the simulations.R script. All 8 scenarios (represented by the 8 panels in Figure 3) must be run to reproduce all data needed for the tables and figures. Use of a cluster is recommended.

The data example cannot be re-run as the data cannot be shared. However, results from the data example are saved in the data_example_results directory, and the following figures and table can be reproduced: Figure 4, Table 1, Figures A.3, A.4, and A.5, and the large table in Section C of the supplementary material. All these figures and tables related can be reproduced by running the script data_example_figures_and_tables.R.
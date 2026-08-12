# Treatment-Label Swapping for Causal Inference

This repository contains R code for a simulation study of **multi-arm treatment-label swapping for causal inference**.

The proposed method swaps treatment labels within causal strata to reduce disclosure risk while preserving the statistical utility of causal effect estimation.

## Methods

The simulation compares:

* Original data
* Proposed treatment-label swapping
* Random swapping
* PRAM
* Randomized response
* Synthetic treatment assignment
* Differentially private randomized response

Causal effects are estimated using:

* IPW
* AIPW
* TMLE

## Simulation Settings

The simulation considers different:

* Sample sizes
* Numbers of covariates
* Covariate correlations
* Numbers of treatment groups

Both **causal estimation accuracy** and **disclosure risk** are evaluated.

## Required R Packages

r
c("MASS", "nnet", "dplyr", "tidyr", "purrr", "stringr")


## Running the Code

Run the R script in R or RStudio:

r
source("simulation.R")


Replace `simulation.R` with the actual filename if necessary.

## Output

Results are saved automatically in the:

text
simulation_results/


folder.

The output includes treatment-effect estimates, accuracy measures, information-preservation measures, and disclosure-risk diagnostics.

## Reproducibility

The simulation uses:

r
set.seed(2026)


## Citation

If you use this code, please cite the associated manuscript.

Citation information will be added after publication.

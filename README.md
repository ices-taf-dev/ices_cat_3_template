2022_ple.27.7e_assessment
================

## Plaice (*Pleuronectes platessa*) in Division 7.e (western English Channel) - WGCSE 2022 (not 2023).

This repository recreates the stock assessment for plaice (*Pleuronectes
platessa*) in Division 7.e (western English Channel) in `R` from WGCSE
2022 - not yet updated for 2023.

## R packages

The following R packages from CRAN are required to run the assessment:

``` r
icesTAF
```

Furthermore, the following packages from GitHub are required:

``` r
cat3advice
```

They can be installed via:

``` r
install.packages("icesTAF")
# install missing packages
install.deps(repos = c("https://cloud.r-project.org", "https://ices-tools-prod.r-universe.dev"))
```

## Running the assessment

The easiest way to run the assessment is to clone or download this
repository, navigate into the repository with R and run:

``` r
### load the icesTAF package
library(TAF)
### load data and install R packages
taf.boot()
### run all scripts
sourceAll()
```

This code snippet runs the data compilation and assessment and creates
the tables and figures presented in the WG report.

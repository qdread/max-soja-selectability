# max x soja Selectability Analysis

[![DOI](https://zenodo.org/badge/475462607.svg)](https://zenodo.org/badge/latestdoi/475462607)

This repo contains all code and data required to reproduce the progeny selectability analysis presented in the manuscript:

Taliercio, E., Eickholt, D., Read, Q. D., Carter, T., Waldeck, N., and Fallen, B. 2022. The impacts of parental choice and seed size on the quality of progeny derived from crosses between *Glycine max* and *Glycine soja*. In preparation.

Note that additional analysis is described in the manuscript (regression to describe the relationship between seed size class and frequency of erect plants) done in SAS 9.4 that is not included here.

*A link to the manuscript and a permanent DOI for this repository will be provided when the manuscript is published.*

## Instructions

All data are included in this repo in the `data/` folder.

The entire procedure, including reading and processing data, fitting models, extracting results from the fit object, and producing figures and tables, is included in the RMarkdown document `soybean_cross_selectability.Rmd`.

The following packages are required: `data.table`, `readxl`, `ggplot2`, `tidyr`, `brms`, `emmeans`, `tidybayes`, `ggtest`, `bayestestR`, and `effectsize`. In addition, a package created by the authors, `Rutilitybelt`, can be installed by calling `remotes::install_github('qdread/Rutilitybelt)`.

To fit models with `brms`, the `cmdstanr` package is needed, as well as an installation of CmdStan software. See <https://mc-stan.org/cmdstanr/> for installation instructions. 

The code in this repo was last tested on 29 March 2022 on R 4.1.2, Windows 10.
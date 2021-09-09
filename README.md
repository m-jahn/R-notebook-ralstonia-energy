# R-notebook-ralstonia-energy

Pipelines for data analysis and visualization of the *Ralstonia* energy metabolism

## Overview

This repository contains pipelines for the analysis of the energy metabolism of *Ralstonia eutropha*, also known as *Cupriavidus necator*, a versatile litho-autotrophic bacterium. The repository contains next generation sequencing data obtained from a barcoded transposon library. Data processing visualization is documented in R notebooks (`*.Rmd`).

All care was taken to guarantee scientific accuracy and adhere to good scientific practice in terms of statistics, reproducibility and code documentation. Please report any errors by filing a [github issue](https://github.com/m-jahn/R-notebook-ralstonia-energy/issues) for this repository, or contact michael.jahn@scilifelab.se.

## How to run the pipelines

Data and pipelines collected in this repository are self-contained and executable. The code _and_ the documentation are part of one and the same R markdown document for each pipeline. The pipelines themselves can be downloaded and executed from the `pipeline` sub-folder. To simply view the rendered pipelines follow the links to the `*.html` reports under [Pipelines](#Pipelines).

To download the repository on your local drive use `git clone` in a (linux) terminal:

``` bash
cd /your-target-folder
git clone https://github.com/m-jahn/R-notebook-ralstonia-energy
```

Open a pipeline with Rstudio and execute code (chunks) with the `Run` button.
Alternatively, open an interactive R session and render the R markdown pipeline:

``` bash
require(rmarkdown)
rmarkdown::render("pipeline.Rmd")
```

## Data

- `data/barseq/20201222_fru_fitness.Rdata`, competition experiments on fructose
- `data/barseq/20210407_suc_for_fitness.Rdata`, competition experiments on formate and succinate
- `data/barseq/20210624_H2_NO3_fitness.Rdata`, competition experiments on hydrogen and nitrate (anoxic growth)
- `data/ref/Ralstonia_H16_genome_annotation.csv`, table with extensive genome annotation, from [uniprot.org](https://www.uniprot.org/uniprot/?query=proteome:UP000008210)

## Libraries

- `lattice`
- `latticeExtra`
- [`latticetools` from github](https://github.com/m-jahn/lattice-tools)
- `tidyverse` (metapackage)
- `dendextend`
- `colorspace`
- `stringi`

## Pipelines

- [Exploring energy metabolism in R. eutropha](https://m-jahn.github.io/R-notebook-ralstonia-energy/Ralstonia_energy_metabolism.nb.html) using a barcoded transposon library. The library was cultivated in bioreactors with different substrate limitations. The depletion/enrichment of transposon mutants over time was tracked using next generation sequencing. This data was used to estimate the fitness contribution of each gene in each condition. 

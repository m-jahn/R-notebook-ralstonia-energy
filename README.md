# R-notebook-ralstonia-energy

Pipelines for data analysis and visualization of the Ralstonia energy metabolism


### Overview

This repository contains pipelines for the analysis of the energy metabolism of *Ralstonia eutropha*, also known as *Cupriavidus necator*, a versatile litho-autotrophic bacterium. The repository contains next generation sequencing data obtained from a barcoded transposon library. Data processing visualization is documented in R notebooks (`*.Rmd`).

All care was taken to guarantee scientific accuracy and adhere to good scientific practice in terms of statistics, reproducibility and code documentation. Please report any errors by filing a [github issue](https://github.com/m-jahn/R-notebook-ralstonia-proteome/issues) for this repository, or contact michael.jahn@scilifelab.se.

### How to run the pipelines

Data and pipelines collected in this repository are (to the most extent) self-contained and executable. The code _and_ the documentation are part of one and the same R markdown document for each pipeline. The pipelines themselves can be downloaded and executed from the `pipeline` sub-folder. To simply view the rendered pipelines follow the links to the `*.html` reports under [Contents](#Contents).

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

### Contents

Links will follow soon.

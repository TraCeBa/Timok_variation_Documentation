# Under the magnifying glass. Dimensions of variation in the contemporary Timok variety
# Documentation

This repository contains R documentation for the quantitative analysis described inthe paper "Under the magnifying glass. Dimensions of variation in the contemporary Timok variety".

The source code is written as R markdown file, stored in the file R_documentation.Rmd. The readable version of this file is either the PDF output (R_documentation.pdf), which can be opened directly here or locally, as well as the HTML output (R_documentation.html) which can be opened in an Internet browser or accessed online [here](https://rpubs.com/tevuko/636831).

The directory contains the following files:

* R markdown (.Rmd) file with all the procedures and references to the files containing quantitative data used in the analyses
* .csv files containing quantitative data resulting from the corpus analyses used in the study
* .xlsx files containing examples and quantitative data resulting from the corpus analyses used in the study
* HTML output of the R markdown file (also available [here](https://rpubs.com/tevuko/636831))
* PDF output of the R markdown file
* preamble.tex file necessary for generating the PDF output

Note that some pieces of code have been hidden from the output files to improve readability. Full code is available in the .Rmd file.

## Prerequisites for opening and running the .Rmd file:

### R and RStudio 

* [R](https://www.r-project.org), a programming language and "a free software environment for statistical computing and graphics" 
* [RStudio](https://rstudio.com/products/rstudio/), an integrated development environment for R, available freely in desktop and server version.

### R packages

```knittr``` package is required for accessing and using the file. Install it by running ```install.packages("knittr")``` in the console.

Other packages specified in the preamble of the .Rmd file are used for the quantitative processing.
```r
library(ggplot2)
library(ggrepel)
library(ggmosaic)
library(gridExtra)
library(tidyverse)
library(reshape)
library(vcd)
library(viridis)
library(plyr)
library(dplyr)
library(leaflet)
```

### For PDF output

Install an application for preparing [LaTeX](https://en.wikipedia.org/wiki/LaTeX) files, such as [MiKTeX](https://miktex.org/download)

Install the ```tinytex``` package by running ```install.packages("tinytex")``` package and load it by running ```library(tinytex)``` (the latter is already included in the preamble of the .Rmd file).

To include HTML objects such as Leaflet maps in PDF, the following are required (already in the preamble of the .Rmd file):

library(webshot)
webshot::install_phantomjs()

**To install the necessary packages listed above, enter the code below (put package name between quotes) in the console:**

```r
install.packages("package name")
```

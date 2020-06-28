
<!-- README.md is generated from README.Rmd. Please edit that file -->

# oisst

<!-- badges: start -->

<!-- badges: end -->

The goal of `oisst` is to easily download [Optimum Interpolation Sea
Surface Temperature (OISST)](https://www.ncdc.noaa.gov/oisst) data
hosted by National Oceanic and Atmospheric Administration (NOAA).

## Installation

``` r
remotes::install_github("andybeet/oisst")
```

## Usage

To download a single years data (year 2001 in example) into a folder
called “output” within your current directory

    oisst::get_oisst_data(years=2001,outputStructure=NULL,outputDir=here::here("output"))

To download years 2000, …, 2010 into yearly folders within the “output”
folder in current working directory:

    oisst::get_oisst_data(years=2000:2010,outputStructure="year",outputDir=here::here("output"))

To download years 2000, …, 2005 into a single folder within the “output”
folder in current working directory:

    oisst::get_oisst_data(years=2000:2005,outputStructure=NULL,outputDir=here::here("output"))

To download all data into monthly folders within the “output” folder in
current working directory:

    ooist::get_oisst_data(years=NULL,outputStructure="month",outputDir=here::here("output"))

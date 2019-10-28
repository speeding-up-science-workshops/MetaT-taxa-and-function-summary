# speeding up science metatranscriptomics heatmap and stacked bar plot visualization 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zeyaxue/speeding-up-sci-heatmap-barplot/master)  

## Summary
Visualization codes from the first "speeding up science workshop". This repository contains codes to make heatmap and stacked bar plots for metatranscriptomic function and RNA-based taxonomy summaries. The demonstration shown here is using data from [this paper](https://aem.asm.org/content/84/1/e02026-17.short) by [Michael D. Lee](https://orcid.org/0000-0001-7750-9145).

## Quick Start
- Once the [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zeyaxue/speeding-up-sci-heatmap-barplot/master) is starxted, user will enter a virtual Rstudio interface. 
- User can either excute the codes with included samples by clicking on the "function-summary.Rmd" and "taxa-summary.rmd" scripts or upload new data files by clicking the `Upload` button at the xxx .

## Example Input
#### 1. A count table with either gene or taxonomy profile per sample. 
If the user want to normalize the count table, user can run the "raw-to-TPM-conversion.R" script.

|       | CDS_ID     | Low_A     | Low_B    | High_A   | High_B   |
|------:|:-----------|-----------|----------|---------:|---------:|
|     0 |    CDS_100 | 10.980509 | 8.364332 | 28.15585 | 0.000000 |
|     1 |  CDS_10011 |  2.284764 | 1.522854 | 10.25240 | 0.000000 |
|     2 |  CDS_10013 |  9.833839 | 6.554506 |  0.00000 | 0.000000 |
|     3 |  CDS_10015 |  7.194288 | 2.501831 |  0.00000 | 0.000000 |
|     4 |  CDS_10016 |  0.000000 | 0.000000 | 44.98916 | 0.000000 |

-   A annotation or taxonomy table

<!-- -->

    ##      CDS_ID KO_ID  Domain        Phylum           Class              Order
    ## 1  CDS_2383  <NA> Archaea Euryarchaeota    Methanococci    Methanococcales
    ## 2  CDS_4184  <NA> Archaea Euryarchaeota Methanomicrobia  Methanosarcinales
    ## 3  CDS_6601  <NA> Archaea Euryarchaeota Methanomicrobia  Methanosarcinales
    ## 4  CDS_6904  <NA> Archaea Euryarchaeota    Methanococci    Methanococcales
    ## 5  CDS_7927  <NA> Archaea Euryarchaeota    Halobacteria       Natrialbales
    ## 6 CDS_15355  <NA> Archaea Euryarchaeota Methanomicrobia Methanomicrobiales
    ##                  Family              Genus                     Species
    ## 1 Methanocaldococcaceae Methanocaldococcus Methanocaldococcus_infernus
    ## 2    Methanosarcinaceae     Methanosarcina      Methanosarcina_barkeri
    ## 3    Methanosarcinaceae     Methanosarcina      Methanosarcina_barkeri
    ## 4      Methanococcaceae      Methanococcus     Methanococcus_vannielii
    ## 5         Natrialbaceae      Haloterrigena      Haloterrigena_jeotgali
    ## 6   Methanomicrobiaceae     Methanolacinia  Methanolacinia_petrolearia

-   A sample metainfo tablex

<!-- -->

    ##   SampleID Place Group
    ## 1   High_A  High     A
    ## 2   High_B  High     B
    ## 3    Low_A   Low     A
    ## 4    Low_B   Low     B





-   Written by Zhengyao "Zeya" Xue, [ORCID](https://orcid.org/0000-0002-4930-8212)
-   The data files and R scripts can be found in this [GitHub repo](https://github.com/zeyaxue/speeding-up-science-binder)
-   [Launch Binder](https://mybinder.org/v2/gh/zeyaxue/speeding-up-science-binder/master?urlpath=rstudio)
-   [html version](https://github.com/zeyaxue/speeding-up-science-binder/blob/master/taxa-summary.md)

-   Thumbnail of expected Heatmap

<img src="https://raw.githubusercontent.com/zeyaxue/speeding-up-sci-heatmap-barplot/master/figs/taxa_heat_thumb.png" width="50%" />

-   Thumbnail of expected bar plot

<img src="https://raw.githubusercontent.com/zeyaxue/speeding-up-sci-heatmap-barplot/master/figs/taxa_bar_thumb.png" width="50%" />



Introduction
------------




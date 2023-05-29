# Antarctic penguin analysis

## Introduction

This is the repository associated with the analysis project titled "Penguins at Palmer Station, Antarctica". In this analysis, we asked:  
1) how male and female Adelie penguins differ in flipper length,  
2) how penguin bill length predicts bill width, and  
3) what set of variables best predict penguin body mass.

## Data and file overview

This repository is organized as follows:

```
.
├── ENVS-193DS_example-repo.Rproj
├── README.md
├── code                                          # all analysis files
│   └── final_project.qmd
└── data                                          # all data files, including accession information
    ├── knb-lter-pal.219.5                              # Adelie
    │   ├── knb-lter-pal.219.5.report.xml
    │   ├── knb-lter-pal.219.5.txt
    │   ├── knb-lter-pal.219.5.xml
    │   ├── manifest.txt
    │   └── table_219.csv
    ├── knb-lter-pal.220.7                              # Chinstrap
    │   ├── knb-lter-pal.220.7.report.xml
    │   ├── knb-lter-pal.220.7.txt
    │   ├── knb-lter-pal.220.7.xml
    │   ├── manifest.txt
    │   └── table_220.csv
    └── knb-lter-pal.221.8                              # Gentoo
        ├── knb-lter-pal.221.8.report.xml
        ├── knb-lter-pal.221.8.txt
        ├── knb-lter-pal.221.8.xml
        ├── manifest.txt
        └── table_221.csv
```

The final rendered report is [here]().

## Sharing and accessing information

This repository and the associated analysis are examples of expectations for the ENVS 193DS final.

We used the `penguins` data set in the `{palmerpenguins}` package:

Horst AM, Hill AP, Gorman KB (2020). palmerpenguins: Palmer Archipelago (Antarctica) penguin data. R package version 0.1.0. <https://allisonhorst.github.io/palmerpenguins/>. doi: [10.5281/zenodo.3960218](https://allisonhorst.github.io/palmerpenguins/index.html).

The data were originally published in:

Gorman KB, Williams TD, Fraser WR (2014). Ecological sexual dimorphism and environmental variability within a community of Antarctic penguins (genus Pygoscelis). PLoS ONE 9(3):e90081. <https://doi.org/10.1371/journal.pone.0090081>.  

We downloaded the raw data from the Environmental Data Initiative portal.  

Palmer Station Antarctica LTER and K. Gorman. 2020. Structural size measurements and isotopic signatures of foraging among adult male and female Adélie penguins (Pygoscelis adeliae) nesting along the Palmer Archipelago near Palmer Station, 2007-2009 ver 5. Environmental Data Initiative. https://doi.org/10.6073/pasta/98b16d7d563f265cb52372c8ca99e60f (Accessed 2023-05-29).  

Palmer Station Antarctica LTER and K. Gorman. 2020. Structural size measurements and isotopic signatures of foraging among adult male and female gentoo penguins (Pygoscelis papua) nesting along the Palmer Archipelago near Palmer Station, 2007-2009 ver 7. Environmental Data Initiative. https://doi.org/10.6073/pasta/9fc8f9b5a2fa28bdca96516649b6599b (Accessed 2023-05-29).  

Palmer Station Antarctica LTER and K. Gorman. 2020. Structural size measurements and isotopic signatures of foraging among adult male and female Chinstrap penguins (Pygoscelis antarcticus) nesting along the Palmer Archipelago near Palmer Station, 2007-2009 ver 8. Environmental Data Initiative. https://doi.org/10.6073/pasta/ce9b4713bb8c065a8fcfd7f50bf30dde (Accessed 2023-05-29).

## Methodologial information

We explored and wrangled the data using `{tidyverse}`. We summarized test results in tabular form using the `{flextable}` package.

## Data-specific information

The data are as follows:

|     Variable             |   Type          |   Description                           |
|--------------------------|-----------------|-----------------------------------------|
|    `species`             |   categorical   |   Adelie, Chinstrap, Gentoo             |
|    `island`              |   categorical   |   Torgersen, Dream, Biscoe              |
|    `bill_length_mm`      |   numerical     |   penguin bill length measured in mm    |
|    `bill_depth_mm`       |   numerical     |   penguin bill depth measured in mm     |
|    `flipper_length_mm`   |   numerical     |   penguin flipper length measured in mm |
|    `body_mass_g`         |   numerical     |   penguin body mass measured in g       |
|    `sex`                 |   categorical   |   male, female                          |
|    `year`                |   categorical   |   2007, 2008, 2009                      |

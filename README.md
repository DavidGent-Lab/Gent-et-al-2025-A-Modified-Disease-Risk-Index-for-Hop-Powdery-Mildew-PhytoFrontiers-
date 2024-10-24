## Gent-et-al-2025-A-Modified-Disease-Risk-Index-for-Hop-Powdery-Mildew-PhytoFrontiers-
This repository contains data and SAS code needed to reproduce the analysis presented in Gent et al. 2025, submitted to PhytoFrontiers. The data set is from five years of experiments conducted to: (1) field validate a modified risk index for the foliar phase of hop powdery mildew and (2) understand the impact of varying the date of the final fungicide application of the year on the cone phase of the disease. Experiments were conducted in Washington State during 2020 to 2023 and 2018 to 2022, respectively.

These files are provided to enable full reproducibility of the statistical analysis presented in the paper. We make no warranties regarding these programs.

Corresponding author: David H. Gent dave.gent@usda.gov

# Files

Four data sets are provided as .csv files. Note that period symbols indicate data was missing or not relevant for a given factor.
(1) Interval: Field data for validation of the modified risk index during 2020 to 2022.
(2) Index: Data used for post-hoc analysis of the modified powdery mildew risk index.
(3) Cascade: Data on cone quality factors from the late-season fungicide timing experiments during 2018 to 2022.
(4) Mildew: Data on levels of disease on the cones in the late-season fungicide timing experiments during 2018 to 2022.

Three text files are provided that contain both the data referenced above and SAS version 9.4 code to reproduce the analyses. These are files are:
(1) SAS Code 2020 to 2023 Field Validation Studies for Modifed Powdery Mildew Risk Index.text
(2) SAS Code Post Hoc Analysis of Modified Risk Index
(3) SAS Code 2018 to 2022 Late Season Disease Control

The file names should be self-explantory.

# Variable Description

Variable names in the data set are as follows for the four data sets.

## Interval

Year: Year the experiment was conducted; ranges from 2020 to 2023.

Site: Location where the experiment was conducted, either Toppenish or Prosser. 

DATE: Date of leaf disease assessment in M/D/YYYY format.

SU: Sampling unit, which is always indicated as Leaf.

REP: Replicate block; Roman numerals indicate replication (block) I to VII.

TRT: Fungicide treatment; 1 = 10-day interval, 2 = 14-day interval, 3 = 21-day interval, and 4 = risk index.

PLANT: Plant number within each plot, ranging from 1 to 10.

PM: The number of leaves (out of 10 evaluated) with powdery mildew.


## Index

Year: Year evaluated; ranges from 2016 to 2022

State: Oregon (OR) or Washington (WA)

Station: Name of AgWeatherNet weather station from which weather data was retrieved.

PMI: Version of the powdery mildew risk index evaluated. 30C is the original indes. 28C is a version that has a lower high temperature threshold. 28C_4C is a version that has both the lower high temperature threshold and a 4C low temperature rule;
The PMI indicated as 28C_4C_4h is a more conservative version that was evaluated but not presented or discussed in the paper;

Sprays: Number of fungicide applications recommended by the various indexes. Analyses involving this output variable were not included in the paper because they are redudant to Interval or Mean index value.

Interval: Mean application interval for a given version of a risk over the period of observations.

MeanIndex: Mean value of a given version of a risk over the period of observation.

MedianIndex: Median value of a given version of a risk over the period of observation. Note used directly in the analyses reported here.

Std: Standard deviation of the index within the given year x station. Note used directly in the analyses reported here.

## Cascade
Year: Year evaluated; ranges from 2018 to 2022

Date: Date of cone harvest in M/D/YYYY format.

Field: Indicator of hop yard where plot was located.

Block: Replicate block; Roman numerals indicate replication (block) I to VII.

Treatment: Values of 1 to 4 corresponding to the date of the last fungicide application: 1 is ceasing at bloom, 2 is bloom + one addition, 3 is bloom + two additional, and 4 is bloom + three additional

Dry_Matter: Percent dry matter

A_acid: Percent alpha-acids, adjusted to 8% moisture

B_acid: Percent beta-acids, adjusted to 8% moisture

_HSI: Hop Storage Index, continuous values

Color: Cone color, rating on a 1 to 10 scale

## Mildew
YEAR: Year evaluated; ranges from 2018 to 2022

DATE: Date of cone harvest in M/D/YYYY format.

SU: Sampling unit, which is always indicated as Cone.

REP: Replicate block; Roman numerals indicate replication (block) I to VII.

TRT:	Values of 1 to 4 corresponding to the date of the last fungicide application: 1 is ceasing at bloom, 2 is bloom + one addition, 3 is bloom + two additional, and 4 is bloom + three additional

PLANT: Plant number within each plot, ranging from 1 to 10.

PM: The number of cones (out of 10 evaluated) with powdery mildew.


## Other Notes
Some additional code is provided for basic data visualization or summary which were not published in the paper.

# Reproduction: Connections between present-day water access and historical redlining

### Authors

- Jorre Dahl, jdahl@middlebury.edu, @jorredahl, Middlebury College
- Lucas Nerbonne, lnerbonne@middlebury.edu, @lnerbonne, Middlebury College

### Abstract

This study is a *reproduction* of Charles W. Sterling III et al's study on "Connections Between Present-Day Water Access and Historical Redlining":

> Sterling III, Charles W., et al. "Connections between present-day water access and historical redlining." Environmental Justice (2023). [doi.org/10.1089/env.2022.0115](https://doi.org/10.1089/env.2022.0115)

This study uses ACS Census data and historical HOLC records of neighborhoods to examine the correlation of historical redlining and current-day access to water in cities. The study uses a binary logistic regression to identify relationships of different demographic and HOLC varaibles to access to water and sewage. The study finds that historically worse HOLC scores were correlated with less access to water in cities across all regions of the United States.

### Study metadata

- `Key words`: Comma-separated list of keywords (tags) for searchability. Geographers often use one or two keywords each for: theory, geographic context, and methods.
- `Subject`: select from the [BePress Taxonomy](http://digitalcommons.bepress.com/cgi/viewcontent.cgi?article=1008&context=reference)
- `Date created`: date when project was started
- `Date modified`: date of most recent revision
- `Spatial Coverage`: Specify the geographic extent of your study. This may be a place name and link to a feature in a gazetteer like GeoNames or OpenStreetMap, or a well known text (WKT) representation of a bounding box.
- `Spatial Resolution`: Specify the spatial resolution as a scale factor, description of the level of detail of each unit of observation (including administrative level of administrative areas), and/or or distance of a raster GRID size
- `Spatial Reference System`: Specify the geographic or projected coordinate system for the study, e.g. EPSG:4326
- `Temporal Coverage`: Specify the temporal extent of your study---i.e. the range of time represented by the data observations.
- `Temporal Resolution`: Specify the temporal resolution of your study---i.e. the duration of time for which each observation represents or the revisit period for repeated observations
- `Funding Name`: name of funding for the project
- `Funding Title`: title of project grant
- `Award info URI`: web address for award information
- `Award number`: award number

#### Original study spatio-temporal metadata

- `Spatial Coverage`: extent of original study
- `Spatial Resolution`: resolution of original study
- `Spatial Reference System`: spatial reference system of original study
- `Temporal Coverage`: temporal extent of original study
- `Temporal Resolution`: temporal resolution of original study

## Study design

This study is a reproduction of a previous study. However, while the previous study did not directly publish their code, and used Python, R and ArcGIS to complete their methods, all methods in this study will be written and published in a single R Markdown script, so that the results are available for others that wish to reproduce this study.

## Materials and procedure

### Computational environment

This study will be done in R Studio Version 2024.12.1, using the: packages.

### Data and variables

Describe the **data sources** and **variables** to be used.
Data sources may include plans for observing and recording **primary data** or descriptions of **secondary data**.
For secondary data sources with numerous variables, the analysis plan authors may focus on documenting only the variables intended for use in the study.

Primary data sources for the study are to include ... .
Secondary data sources for the study are to include ... .

Each of the next subsections describes one data source.

#### Primary data source1 name

**Standard Metadata**

- `Abstract`: Brief description of the data source
- `Spatial Coverage`: Specify the geographic extent of your study. This may be a place name and link to a feature in a gazetteer like GeoNames or OpenStreetMap, or a well known text (WKT) representation of a bounding box.
- `Spatial Resolution`: Specify the spatial resolution as a scale factor, description of the level of detail of each unit of observation (including administrative level of administrative areas), and/or or distance of a raster GRID size
- `Spatial Reference System`: Specify the geographic or projected coordinate system for the study
- `Temporal Coverage`: Specify the temporal extent of your study---i.e. the range of time represented by the data observations.
- `Temporal Resolution`: Specify the temporal resolution of your study---i.e. the duration of time for which each observation represents or the revisit period for repeated observations
- `Lineage`: Describe and/or cite data sources and/or methodological steps planned to create this data source.
  - sampling scheme, including spatial sampling
  - target sample size and method for determining sample size
  - stopping criteria for data collection and sampling (e.g. sample size, time elapsed)
  - de-identification / anonymization
  - experimental manipulation
- `Distribution`: Describe who will make the data available and how?
- `Constraints`: Legal constraints for *access* or *use* to protect *privacy* or *intellectual property rights*
- `Data Quality`: State any planned quality assessment
- `Variables`: For each variable, enter the following information. If you have two or more variables per data source, you may want to present this information in table form (shown below)
  - `Label`: variable name as used in the data or code
  - `Alias`: intuitive natural language name
  - `Definition`: Short description or definition of the variable. Include measurement units in description.
  - `Type`: data type, e.g. character string, integer, real
  - `Accuracy`: e.g. uncertainty of measurements
  - `Domain`: Expected range of Maximum and Minimum of numerical data, or codes or categories of nominal data, or reference to a standard codebook
  - `Missing Data Value(s)`: Values used to represent missing data and frequency of missing data observations
  - `Missing Data Frequency`: Frequency of missing data observations: not yet known for data to be collected

| Label | Alias | Definition | Type | Accuracy | Domain | Missing Data Value(s) | Missing Data Frequency |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| variable1 | ... | ... | ... | ... | ... | ... | ... |
| variable2 | ... | ... | ... | ... | ... | ... | ... |

#### Primary data source2 name

... same form as above...

#### Secondary data source1 name

**Standard Metadata**

- `Abstract`: Brief description of the data source
- `Spatial Coverage`: Specify the geographic extent of your study. This may be a place name and link to a feature in a gazetteer like GeoNames or OpenStreetMap, or a well known text (WKT) representation of a bounding box.
- `Spatial Resolution`: Specify the spatial resolution as a scale factor, description of the level of detail of each unit of observation (including administrative level of administrative areas), and/or or distance of a raster GRID size
- `Spatial Reference System`: Specify the geographic or projected coordinate system for the study
- `Temporal Coverage`: Specify the temporal extent of your study---i.e. the range of time represented by the data observations.
- `Temporal Resolution`: Specify the temporal resolution of your study---i.e. the duration of time for which each observation represents or the revisit period for repeated observations
- `Lineage`: Describe and/or cite data sources and/or methodological steps used to create this data source
- `Distribution`: Describe how the data is distributed, including any persistent identifier (e.g. DOI) or URL for data access
- `Constraints`: Legal constraints for *access* or *use* to protect *privacy* or *intellectual property rights*
- `Data Quality`: State result of quality assessment or state "Quality unknown"
- `Variables`: For each variable, enter the following information. If you have two or more variables per data source, you may want to present this information in table form (shown below)
  - `Label`: variable name as used in the data or code
  - `Alias`: intuitive natural language name
  - `Definition`: Short description or definition of the variable. Include measurement units in description.
  - `Type`: data type, e.g. character string, integer, real
  - `Accuracy`: e.g. uncertainty of measurements
  - `Domain`: Range (Maximum and Minimum) of numerical data, or codes or categories of nominal data, or reference to a standard codebook
  - `Missing Data Value(s)`: Values used to represent missing data and frequency of missing data observations
  - `Missing Data Frequency`: Frequency of missing data observations

| Label | Alias | Definition | Type | Accuracy | Domain | Missing Data Value(s) | Missing Data Frequency |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| variable1 | ... | ... | ... | ... | ... | ... | ... |
| variable2 | ... | ... | ... | ... | ... | ... | ... |

#### Secondary data source2 name

... same form as above...

### Prior observations  

There are o prior observations related with this data.

### Bias and threats to validity

The two main source of bias in this study come from the HOLC data itself. Firstly, the spatial extent of the HOLC data only covers the centers of major cities across the united states, limiting the analysis to center-cities. Secondly, Areal Interpolation was used to determine a HOLC grade for each block group, meaning that while a single grade can be determined, there may be some errors in block groups crossing over historic neighborhood boundaries.

### Data transformations

Describe all data transformations planned to prepare data sources for analysis.
This section should explain with the fullest detail possible how to transform data from the **raw** state at the time of acquisition or observation, to the pre-processed **derived** state ready for the main analysis.
Including steps to check and mitigate sources of **bias** and **threats to validity**.
The method may anticipate **contingencies**, e.g. tests for normality and alternative decisions to make based on the results of the test.
More specifically, all the **geographic** and **variable** transformations required to prepare input data as described in the data and variables section above to match the study's spatio-temporal characteristics as described in the study metadata and study design sections.
Visual workflow diagrams may help communicate the methodology in this section.

Examples of **geographic** transformations include coordinate system transformations, aggregation, disaggregation, spatial interpolation, distance calculations, zonal statistics, etc.

Examples of **variable** transformations include standardization, normalization, constructed variables, imputation, classification, etc.

Be sure to include any steps planned to **exclude** observations with *missing* or *outlier* data, to **group** observations by *attribute* or *geographic* criteria, or to **impute** missing data or apply spatial or temporal **interpolation**.

### Analysis

Describe the methods of analysis that will directly test the hypotheses or provide results to answer the research questions.
This section should explicitly define any spatial / statistical *models* and their *parameters*, including *grouping* criteria, *weighting* criteria, and *significance thresholds*.
Also explain any follow-up analyses or validations.

## Results

Data is presented as 3 figures, 2 tables, and 7 supplementary tables:

Figures:

- Map of HOLC grades for different cities across regions
- Correlation plot for potential predictive variables
- Map of percent of houses with incomplete plumbing  across regions

Tables:

- Average Marginal Effects of Variables determined by Binary Regression Model
- The Number of Each Grade Polygon in Each Data Set

Supplementary Tables:

- The results of the Dunn Test to determine whether incomplete plumbing % in Grade A is significantly different than the other Grades
- The average % for each predictive variable broken down by HOLC grade and region
- AME Table for the Nation using the average 2.61168 as the threshold for the binary variable
National
- AME Table for the Northeast region using the average 3.414391 as the threshold for the binary variable
- AME Table for the South region using the average 3.414391 as the threshold for the binary variable
- AME Table for the Midwest region using the average 3.414391 as the threshold for the binary variable
- AME Table for the West region using the average 3.414391 as the threshold for the binary variable

## Discussion

Describe how the results are to be interpreted *vis a vis* each hypothesis or research question.

## Integrity Statement

Include an integrity statement - The authors of this preregistration state that they completed this preregistration to the best of their knowledge and that no other preregistration exists pertaining to the same hypotheses and research.
If a prior registration *does* exist, explain the rationale for revising the registration here.

## Acknowledgements

- `Funding Name`: name of funding for the project
- `Funding Title`: title of project grant
- `Award info URI`: web address for award information
- `Award number`: award number

This report is based upon the template for Reproducible and Replicable Research in Human-Environment and Geographical Sciences, DOI:[10.17605/OSF.IO/W29MQ](https://doi.org/10.17605/OSF.IO/W29MQ)

## References

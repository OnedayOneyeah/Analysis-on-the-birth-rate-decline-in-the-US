# Analysis on the birth rate decline in the US
## Overview
This repository is for the replication of The Puzzle of Falling US Birth Rates Since the Great Recession (Melissa S. Kearney, Phillip B. Levine, and Luke Pardue, 2022). The Input folder includes the datasets manipulated in the paper and a bibTex file used for a bibliography in RMarkdown file. The output folder consists of RMarkdown file with the exported pdf file, and the log file. Finally, RScript cleaning the input datasets is included in Script folder.

## Comupational Requirements
To run the codes in RMarkdown and RScript file, R[[1]](#1) is required to be installed. Related R packages should be installed before running the codes as well, and it is acheivable by running codes in 'computational_requirements.R' file in this repository. We used tidyverse[[2]](#2) to manipulate the datasets, knitr[[3]](#3) and kableExtra[[4]](#4) to generate tables with the cleaned datasets and fix its placement in the paper. usmap[[5]](#5) helped to plot datasets on US map, generating related figures. Finally, bookdown[[6]](#6) was used as a powerful cross referene tool for generating final pdf document. 

## Data Availability and Provenance Statements
### Statement about Rights
I certify that the author(s) of the manuscript have legitimate access to and permission to use the data used in this manuscript.

### Summary of availability
All data in the replication package is available here.

### Details on data files
All the figures and tables in the replication paper were created with five datasets in 'Input/Data' in total. The datasets are listed below.

|Data file|Figure/Table|Notes|Provided|
|---|---|---|---|
|fig_1.csv|Figure 1, Table2|The US Birth Rate from 1980 to 2020|Yes|
|figs_2a_2b.csv|Figure 2, Table 3, Figure 3|The US Birth Rate by Age Group, Race and Ethnicity|Yes|
|fig_7.csv|Figure 4, Figure 5.2|Change in Birth Rate by State between 2004-2008 and 2015-2019 (15-44)|Yes|
|hispanic.csv|Table 4|Hispanic population data by State (2022)|Yes|
|numbirths_2001_2019.csv|Figure 5.1|The Number of Birth by State by State from 1990 to 2019 (15-44)|Yes|

Here are the heads of each data file.
**1. fig_1.csv**
|year|brate_all|
|---|---|
|1980|68.4|
|1981|67.3|
|1982|67.3|
|1983|65.7|
|1984|65.5|

**2. fig_2a_2b.csv**
|year|brate_1519|brate_2024|brate_2529|brate_3034|brate_3539|brate_4044|brate_whitenh|brate_blacknh|brate_hisp|
|---|---|---|---|---|---|---|---|---|---|
|1980|53|115.1|112.9|61.9|19.8|3.9|   |   |    |
|1981|52.2|112.2|111.5|61.4|20|3.8|   |   |    |
|1982|52.4|111.6|111|64.1|21.2|3.9|   |   |    |
|1983|51.4|107.8|108.5|64.9|22|3.9|   |   |    |
|1984|50.6|106.8|108.7|67|22.9|3.9|   |   |    |

**3. fig_7.csv**
|stname|brate1544_thsnds_ch_pct|
|---|---|
|AK|-5.4787889|
|AL|-5.3939962|
|AR|-7.8527479|
|AZ|-25.359673|
|CA|-18.001598|

**4. hispanic.csv**
|State|WhiteHispanicPerc|BlackHispanicPerc|IndianHispanicPerc|AsianHispanicPerc|HawaiianHispanicPerc|OtherHispanicPerc|
|---|---|---|---|---|---|---|
|Alabama|0.0257|0.0015|0.0006|0.0002|0.0001|0.0147|
|Alaska|0.0395|0.0018|0.0047|0.0014|0.0003|0.0227|
|Arizona|0.2252|0.0029|0.0058|0.0009|0.0002|0.0782|
|Arkansas|0.0429|0.0009|0.0009|0.0002|0.0000|0.0298|
|California|0.2252|0.0027|0.0042|0.0021|0.0004|0.1557|


**5 numbirths_2001_2019.csv**
|year|stname|numbirth1544|
|---|---|---|
|1990|AK|11881|
|1991|AK|11651|
|1992|AK|11698|
|1993|AK|11056|
|1994|AK|10652|

## References

<a id="1">[1]
  R Core Team (2021). R: A language and
  environment for statistical computing. R
  Foundation for Statistical Computing, Vienna,
  Austria. URL https://www.R-project.org/.
</a> 

<a id="2">[2]
  Wickham et al., (2019). Welcome to the
  tidyverse. Journal of Open Source Software,
  4(43), 1686,
  https://doi.org/10.21105/joss.01686
</a>

<a id="3">[3]
  Yihui Xie (2021). knitr: A General-Purpose
  Package for Dynamic Report Generation in R. R
  package version 1.37.
  </a>
  
 <a id="4">[4]
  Hao Zhu (2021). kableExtra: Construct Complex
  Table with 'kable' and Pipe Syntax. R package
  version 1.3.4.
  https://CRAN.R-project.org/package=kableExtra
  </a>
  
  
<a id ="5">[5]
  Paolo Di Lorenzo (2021). usmap: US Maps
  Including Alaska and Hawaii. R package version
  0.5.2. https://CRAN.R-project.org/package=usmap
  </a>
  
 <a id="6">[6]
  Yihui Xie (2021). bookdown: Authoring Books and
  Technical Documents with R Markdown. R package
  version 0.24.
  </a>

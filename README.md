# Analysis on the birth rate decline in the US
## Overview
This repository is for the replication of *The Puzzle of Falling US Birth Rates Since the Great Recession* (Melissa S. Kearney, Phillip B. Levine, and Luke Pardue, 2022). Input folder includes the datasets manipulated in the paper and a bibTex file used for bibliography in RMarkdown file. Output folder consists of the RMarkdown file with the exported pdf file, and the log file. At last, the RScript cleaning the input datasets is included in Script folder.

## Comupational Requirements
To run the codes in RMarkdown and RScript file, R[[1]](#1) is required to be installed. Related R packages should be installed before running the codes as well, and it is acheivable by running codes in 'computational_requirements.R' file in this repository. To analyze datasets, we used tidyverse[[2]](#2)

## Data Availability 
Datasets used to generate figures and tables in the replication paper are listed below.

|Data file|Figure/Table|Notes|Provided|
|---|---|---|---|
|fig_1.csv|Figure 1, Table2|The US Birth Rate from 1980 to 2020|Yes|
|figs_2a_2b.csv|Figure 2, Table 3, Figure 3|The US Birth Rate by Age Group, Race and Ethnicity|Yes|
|fig_7.csv|Figure 4, Figure 5.2|Change in Birth Rate by State between 2004-2008 and 2015-2019 (15-44)|Yes|
|hispanic.csv|Table 4|Hispanic population data by State (2022)|Yes|
|numbirths_2001_2019.csv|Figure 5.1|The Number of Birth by State by State from 1990 to 2019 (15-44)|Yes|

Here are the heads of each datafile.
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

<a id="1">[1]</a> 
R
<a id="2">[2]</a>
Tidyverse

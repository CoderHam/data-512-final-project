# Final Project Plan - Education Statistics

Final Project for DATA512 - Human-Centered Data Science @ University of Washington

Author: Hemant Jain

## Abstract and Motivation

In this project, I intend to analyze, investigate and study the Education data from World Bank. The data contains several indicators of the access and quality of education. Apart from recorded data, it also possesses projected numbers for these. As someone passionate about education, I wish to perform this exploratory research with an open mind in order to find patterns and explanations for them.

Access to education has for long been an important factor in the improvement of the quality of life as well as the economy of a country. While many countries have taken steps to ensure access to education I wish to investigate the success and effects of this. Is there any bias in the data that suggests unfair practices towards people of a certain race, ethnicity, gender and region.

Apart from improving the lifestyle of individuals, education helps people find their purpose in life, encourages inquisitiveness and introspection, motivates people to be better, broads perspective and improves reasoning skills and creativity.

##  Research Questions

While I intend keep an open mind during the study there are a few **Research Questions** I wish to answer:

1. Is there is a correlation between the number of youth not attending school youth and the level of income?
    1. Can the dataset explain why?
2. Does governments change their investment in education based on their annual GDP?
    1. What education sectors does the investment affect and which does it not?
3. What are the factors affecting quality of Learning? Which parts of learning have seen improvements due to recent demands?
    1. Do attendance rates affect the quality of learning?
    2. Has the Math and Science improved in the recent years?


## Data

The [Education Statistics](https://datacatalog.worldbank.org/dataset/education-statistics) dataset being used in this assignment is downloaded from the [World Bank](http://www.worldbank.org/). The dataset sources it's data from:
1.  UIS ([UNESCO Institute for Statistics](http://uis.unesco.org/)) - Administrative country data
2. Several International and Regional learning assessments
3. [World Bank Education Projects Database](http://datatopics.worldbank.org/education/wQueries/qprojects) - activities, components and sub-sectors of WB Education projects since 1998
4. [ World Bank Education Expenditures Database](http://datatopics.worldbank.org/education/wQueries/qexpenditures) - Education expenditure data

The dataset has been downloaded and added to the [`data`](https://github.com/CoderHam/data-512-final-project/tree/master/data) directory and consists of 5 parts that have been described below:

1.  [**EdStatsCountry.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsCountry.csv)

| Column | Datatype | Description |
|---|---|---|
| Country Code |
|	Short Name |
| Table Name |
| Long Name |
| 2-alpha code |
| Currency Unit|
| Special Notes|
| Region |
| Income Group |
| WB-2 code |
| National accounts base year |
| National accounts reference year|
| SNA price valuation|
| Lending category |
| Other groups |
| System of National Accounts|
| Alternative conversion factor|
| PPP survey year|
| Balance of Payments Manual in use|
| External debt Reporting status|
| System of trade|
| Government Accounting concept|
| IMF data dissemination standard|
| Latest population census|
| Latest household survey|
| Source of most recent Income and expenditure data|
| Vital registration complete|
| Latest agricultural census|
| Latest industrial data |
| Latest trade data|
| Latest water withdrawal data|

2. [**EdStatsCountry-Series.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsCountry-Series.csv)

| Column | Datatype | Description |
|---|---|---|
| CountryCode	|
| SeriesCode |
| Description |

3. [**EdStatsData.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsData.csv)

| Column | Datatype | Description |
|---|---|---|
|Country Name|
|Country Code|
|Indicator Name|
|Indicator Code|
|{Year} (1970 to 2017 as with 5 year binned projections till 2100)|

4. [**EdStatsSeries.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsSeries.csv)

| Column | Datatype | Description |
|---|---|---|
|Series Code|
|Topic|
|Indicator Name|
|Short definition|
|Long definition|
|Unit of measure|
|Periodicity|
|Base Period|
|Other notes|
|Aggregation method|
|Limitations and exceptions|
|Notes from original source|
|General comments|
|Source	Statistical concept and methodology|
|Development relevance|
|Related source links|
|Other web links|
|Related indicators|
|License Type|

5. [**EdStatsFootNote.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsFootNote.csv)

| Column | Datatype | Description |
|---|---|---|
| CountryCode|
| SeriesCode|
| Year|
| Description |

## Licenses

The dataset is classified **Public** and is licensed under the [**CC-BY 4.0**](https://datacatalog.worldbank.org/public-licenses#cc-by). A short summary of [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) is that under this license, individuals are free to copy and redistribute data in any medium as well as modify and build upon the data for all purposes including commercially.

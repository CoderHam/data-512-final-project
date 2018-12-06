# Final Project Plan - Education Statistics

Final Project for DATA512 - Human-Centered Data Science @ University of Washington

Author: Hemant Jain

## Abstract and Motivation

Personal motivation: In most developing countries a large portion of the youth does not have access to primary and secondary education even today.

**"In 40 out of 93 countries, fewer than 50% of the poorest children have completed primary school"**.[6]

Without proper education, it is hard for individuals from poor families to  seek employment pays well and rise above the poverty. This in turn affects their quality of life and that of their future generations. It was this passion towards education and it's access for all that led me to join an NGO - [Make a Difference](https://makeadiff.in/) (MAD) during my undergraduate and as a part MAD, I educated and facilitated the education of orphaned and underprivileged children.

In this project, I intend to analyze, investigate and study the Education data from World Bank. The data contains several indicators of the access and quality of education. Apart from recorded data, it also possesses projected numbers for these. As someone passionate about education, I wish to perform this exploratory research with an open mind in order to find patterns and explanations for them.

Access to education has for long been an important factor in the improvement of the quality of life as well as the economy of a country. While many countries have taken steps to ensure access to education I wish to investigate the success and effects of this. Is there any bias in the data that suggests unfair practices towards people of a certain race, ethnicity, gender and region.

Apart from improving the lifestyle of individuals, education helps people find their purpose in life, encourages inquisitiveness and introspection, motivates people to be better, broads perspective and improves reasoning skills and creativity.

##  Research Questions

While I intend keep an open mind during the study there are a few **Research Questions** I wish to answer:

1. Education and Income
    1. Is there is a correlation between the number of youth attending school and the level of income? Focus on verifying the claim:

    **"Children living in a low income countries are twice as likely to be out of school than those children in high income countries. Additionally, children from the wealthiest 20% of the population are 4 times more likely to be in school than the poorest 20%."**[5]

    2. What factors contribute to the lack of students enrolled in schools.
2. Government's role in Education
    1. Does governments change their investment in education based on their annual GDP?
    2. What education sectors does the investment affect and which does it not?
3. Quality of Education
    1. What are the factors affecting such as attendance rates quality of Learning?
    2. Which parts of learning have seen improvements due to recent demands? Has the Math and Science improved in the recent years?
4. Gender
    1. Does gender impact the enrollment, level and quality of education received?

    This article - [Why girls in India are still missing out on the education they need](https://www.theguardian.com/education/2013/mar/11/indian-children-education-opportunities) talks about the problem in India.

    **"India is no longer considered a poor country and yet many children do not receive a good education." - Rachel Williams"**

    I intend to test if this is true for other countries with better/worse economies.

## Human-Centered Design Considerations

I have decided to include the following Human-Centered design considerations:

1. Knowledge of current affairs impacting education
2. Qualitative analysis based on additional data about perceived attitude towards education
3. In the manner of the Research Questions asked in the study
4. Incorporating visualizations and qualitative analysis when possible

## Data (Source and Schema)

The [Education Statistics](https://datacatalog.worldbank.org/dataset/education-statistics) dataset being used in this assignment is downloaded from the [World Bank](http://www.worldbank.org/). The dataset sources it's data from:
1.  UIS ([UNESCO Institute for Statistics](http://uis.unesco.org/)) - Administrative country data
2. Several International and Regional learning assessments
3. [World Bank Education Projects Database](http://datatopics.worldbank.org/education/wQueries/qprojects) - activities, components and sub-sectors of WB Education projects since 1998
4. [ World Bank Education Expenditures Database](http://datatopics.worldbank.org/education/wQueries/qexpenditures) - Education expenditure data

The dataset has been downloaded and added to the [`data`](https://github.com/CoderHam/data-512-final-project/tree/master/data) directory and consists of 5 parts that have been described below:

1.  [**EdStatsCountry.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsCountry.csv)

| Column | Datatype | Description |
|---|---|---|
| Country Code | text | a three digit unique code to represent a country |
| Short Name | text | short name for the country |
| Table Name | text | the name being used in this table |
| Long Name | text | full name of the country |
| 2-alpha code | text | alphanumeric code of length 2 for the country |
| Currency Unit | text | currency of the country |
| Special Notes | text | additional notes about the country |
| Region | text | region where the country is location |
| Income Group | text | which income group the country belongs to |
| WB-2 code | text | World Bank 2 letter code |
| National accounts base year | numeric | base year used for country accounts |
| National accounts reference year| numeric | reference year for the country accounts |
| SNA price valuation| text | System of National Accounts (SNA) valuation of currency |
| Lending category | text | the lending agency for that country as decided by World Bank |
| Other groups | text | other World Bank/UN groups that the country belongs to |
| System of National Accounts| text | the year of SNA methodology the country uses |
| Alternative conversion factor| text | the DEC alternative conversion factor OR the official exchange rate reported by IMF's International Financial Statistics (IFS) |
| PPP survey year| numeric | survey year for the nation's Purchasing power parity (PPP) |
| Balance of Payments Manual in use| text | the IMF balance of payments manual used by the country |
| External debt Reporting status| text | the type of the external debt reported |
| System of trade| text | the type of trade system the nation uses |
| Government Accounting concept| text | the type of accounting the central government uses |
| IMF data dissemination standard| text | the data dissemination standard used by IMF for that nation |
| Latest population census| numeric | the last year the nations population census was reported |
| Latest household survey| text | the last year the nations household survey was reported |
| Source of most recent Income and expenditure data | text |  the source and last year the nations income and expenditure data was reported |
| Vital registration complete | categorical | has the nation completed vital registration |
| Latest agricultural census| numeric | the last year the nations agricultural data was reported |
| Latest industrial data | numeric | the last year the nations industrial data was reported |
| Latest trade data| numeric | the last year the nations trade data was reported |
| Latest water withdrawal data| numeric | the last year the nations water withdrawal data was reported |

2. [**EdStatsCountry-Series.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsCountry-Series.csv)

| Column | Datatype | Description |
|---|---|---|
| CountryCode	| text | a three digit unique code to represent a country |
| SeriesCode | text | the code for the data series |
| Description | text | source of data / estimates |

3. [**EdStatsData.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsData.csv)

| Column | Datatype | Description |
|---|---|---|
|Country Name| text | the name of the country |
|Country Code| text | a three digit unique code to represent a country |
|Indicator Name| text | the name of the indicator being listed |
|Indicator Code| text | the indicator code for the indicator being listed |
|{Value for the Year} (1970 to 2017 as with 5 year binned projections till 2100)| numeric | the value of the indicator for that code |

4. [**EdStatsSeries.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsSeries.csv)

| Column | Datatype | Description |
|---|---|---|
|Series Code| text | the code for the data series |
|Topic| text | topic category the series belongs to |
|Indicator Name| text | name of the indicator |
|Short definition| text | a short definition of the indicator |
|Long definition| text | a detailed definition of the indicator |
|Unit of measure| text | the unit of measure for the indicator |
|Periodicity| numeric | time between successive recordings of for the indicator |
|Base Period| numeric | the year used as reference for the base value for the indicator |
|Other notes| text | additional details about the indicator |
|Aggregation method| text | how the indicator was recorded or inferred |
|Limitations and exceptions| text | details about the limits and expectations for the indicator |
|Notes from original source| text | notes from- the source of the indicator |
|General comments| text | comments about citations or use of this data |
|Source	| text | source of the indicator data |
|Statistical concept and methodology| text | The method or study used to find the value of the indicator |
|Development relevance| text | additional information about the collection of the indicator |
|Related source links| text | link to source of the data |
|Other web links| text | additional links for the data |
|Related indicators| text | related indicators in the dataset |
|License Type| text | license type for the indicator|

5. [**EdStatsFootNote.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/EdStatsFootNote.csv)

| Column | Datatype | Description |
|---|---|---|
| CountryCode| text | a three digit unique code to represent a country |
| SeriesCode| text | the code for the data series |
| Year| numeric | the year for which the data is collected |
| Description | text | the method of collection/estimation of the indicator |

I added data for the current income levels, as classified by World Bank [7].

6. [**income_group.csv**](https://github.com/CoderHam/data-512-final-project/tree/master/data/income_group.csv)

| Column | Datatype | Description |
|---|---|---|
|Economy| text | the name of the country |
| Code| text | a three digit unique code to represent a country |
| Region | text | region where the country is location |
| Income group | text | which income group the country belongs to |
| Lending category | text | the lending agency for that country as decided by World Bank |
| Other | text | other World Bank/UN groups that the country belongs to |


## Licenses

The dataset is classified **Public** and is licensed under the [**CC-BY 4.0**](https://datacatalog.worldbank.org/public-licenses#cc-by). A short summary of [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) is that under this license, individuals are free to copy and redistribute data in any medium as well as modify and build upon the data for all purposes including commercially.


## Data Pre-processing and Preparation

The data is distributed across the 5 csv files and has many missing values, extra details and incorrect formatting. There is no exhaustive description of each column and domain specific phrases and the same must be studied and inferred by referring to relevant literature and the UNIS and World Bank website.

## Considerations for Gender

The dataset treats gender and sex as the same i.e. either male or female and while I do not agree that one should be forced to identify between either of the two, I was unable to find relevant education data for non-binary genders.

Stating this as a limitation of the dataset, I will proceed with this data and look for other sources to enrich the dataset.

## Data Limitations

Apart from the data being reported by multiple agencies to the World Bank Group and the UN, there are several missing values. There is a gender limitation in that the dataset assumes binary gender is also important. The projections in the data are absent in many cases and those that are present may not be accurate.

## Conclusions

There are several claims made online regarding inequality in educations, bias against female education [11] and relation between income and education. I wish to investigate these claims and find other such trends in the dataset.

## References

[1] World Bank Education Statistics Dataset - [https://datacatalog.worldbank.org/dataset/education-statistics](https://datacatalog.worldbank.org/dataset/education-statistics)

[2] UNESCO Institute for Statistics - [http://uis.unesco.org/](http://uis.unesco.org/)

[3] Education Statistics (EdStats) - [http://datatopics.worldbank.org/education/](http://datatopics.worldbank.org/education/)

[4] Education Data Release - [http://uis.unesco.org/en/news/education-data-release-one-every-five-children-adolescents-and-youth-out-school](http://uis.unesco.org/en/news/education-data-release-one-every-five-children-adolescents-and-youth-out-school)

[5] 11 Facts About Education Around the World - [https://www.dosomething.org/us/facts/11-facts-about-education-around-world](https://www.dosomething.org/us/facts/11-facts-about-education-around-world)

[6] World Inequality Database on Education - [https://www.education-inequalities.org/](https://www.education-inequalities.org/)

[7] World Bank Country and Lending and Income Groups - [https://datahelpdesk.worldbank.org/knowledgebase/articles/906519-world-bank-country-and-lending-groups](https://datahelpdesk.worldbank.org/knowledgebase/articles/906519-world-bank-country-and-lending-groups)

[8] What is the DEC conversion factor? - [https://datahelpdesk.worldbank.org/knowledgebase/articles/77935-what-is-the-dec-conversion-factor](https://datahelpdesk.worldbank.org/knowledgebase/articles/77935-what-is-the-dec-conversion-factor)

[9] World Bank Knowledge Base - [https://datahelpdesk.worldbank.org/knowledgebase](https://datahelpdesk.worldbank.org/knowledgebase)

[10] Gender Parity Inde - [https://unstats.un.org/unsd/mdg/Metadata.aspx?IndicatorId=9](https://unstats.un.org/unsd/mdg/Metadata.aspx?IndicatorId=9)

[11] Guardian Article on 'Why girls in India are still missing out on the education they need' - [https://www.theguardian.com/education/2013/mar/11/indian-children-education-opportunities](https://www.theguardian.com/education/2013/mar/11/indian-children-education-opportunities)

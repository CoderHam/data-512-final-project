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
    1. Is there is a correlation between the number of youth not attending school youth and the level of income? Focus on verifying the claim:

    **"Children living in a rural environment are twice as likely to be out of school than urban children. Additionally, children from the wealthiest 20% of the population are 4 times more likely to be in school than the poorest 20%."**[5]

    2. What factors contribute to the lack of students enrolled in schools.
2. Government's role in Education
    1. Does governments change their investment in education based on their annual GDP?
    2. What education sectors does the investment affect and which does it not?
3. Quality of Education
    1. What are the factors affecting such as attendance rates quality of Learning?
    2. Which parts of learning have seen improvements due to recent demands? Has the Math and Science improved in the recent years?
4. Gender
    1. Does gender impact the enrollment, level and quality of education received?

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


## Data Pre-processing and Preparation

The data is distributed across the 5 csv files and has many missing values, extra details and incorrect formatting. There is no exhaustive description of each column and domain specific phrases and the same must be studied and inferred by referring to relevant literature and the UNIS and World Bank website.

## Considerations for Gender

The dataset treats gender and sex as the same i.e. either male or female and while I do not agree that one should be forced to identify between either of the two, I was unable to find relevant education data for non-binary genders.

Stating this as a limitation of the dataset, I will proceed with this data and look for other sources to enrich the dataset.

## Data Limitations

Apart from the data being reported by multiple agencies to the World Bank Group and the UN, there are several missing values. There is a gender limitation in that the dataset assumes binary gender is also important. The projections in the data are absent in many cases and those that are present may not be accurate.

## Conclusions

There are several claims made online regarding inequality in educations, bias towards male education and relation between income and education. I wish to investigate these claims and find other such trends in the dataset.

## References

[1] World Bank Education Statistics Dataset - [https://datacatalog.worldbank.org/dataset/education-statistics](https://datacatalog.worldbank.org/dataset/education-statistics)

[2] UNESCO Institute for Statistics - [http://uis.unesco.org/](http://uis.unesco.org/)

[3] Education Statistics (EdStats) - [http://datatopics.worldbank.org/education/](http://datatopics.worldbank.org/education/)

[4] Education Data Release - [http://uis.unesco.org/en/news/education-data-release-one-every-five-children-adolescents-and-youth-out-school](http://uis.unesco.org/en/news/education-data-release-one-every-five-children-adolescents-and-youth-out-school)

[5] 11 Facts About Education Around the World - [https://www.dosomething.org/us/facts/11-facts-about-education-around-world](https://www.dosomething.org/us/facts/11-facts-about-education-around-world)

[6] World Inequality Database on Education - [https://www.education-inequalities.org/](https://www.education-inequalities.org/)

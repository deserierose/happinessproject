# Happiness Project 

# Overview

The disparity in happiness among countries has been well established by the World Happiness Report, founded in 2012. Their thorough investigation of confounding factors related to happiness scores has provided valuable insights into economic and social trends around the world.

However, the purpose of this analysis is to conduct a deeper investigation into additional indicators that may affect a country’s happiness and to provide a comprehensive view of the data from 2012 to 2022. This analysis offers an up-to-date summary of happiness score trends and aims to provide targeted recommendations for policymakers to improve the quality of life in impoverished nations.


## Project Objective 

* Identify key indicators that have the greatest impact on a country's overall happiness
* Identify trends between indicators and happiness scores
* Provide recommendations for policymakers to improve a country's overall happiness

#### Methodology 

* SQL - queries utilized to clean, organize and prepare data can be found [here](https://github.com/deserierose/happinessproject/blob/d95f15a1977e57aecc3df5295e3adc4cd960720d/happiness-project-notebook.ipynb)
* Python - processes utilized to perform statistical analysis can be found [here](https://github.com/deserierose/happinessproject/blob/d95f15a1977e57aecc3df5295e3adc4cd960720d/happiness-project-notebook.ipynb) 
* Statistical Analysis - Further details on methodology and statistical analysis can be found [here](https://github.com/deserierose/happinessproject/blob/ad9c0e5c66ef2e80e9c5db63da80c52f4031bf32/project-happiness-methodology.ipynb)
* Tableau - an overview interactive dashboard can be downloaded [here](https://public.tableau.com/shared/7Q65C3GCH?:display_count=n&:origin=viz_share_link) 
 
# Data Structure 

The following databases were used to extract various indicator records from 2012 to 2022. Each indicator was categorized within one of five datasets: health, environment, economy, government, and education. A country ID was assigned to each country name to connect datasets. Prior to analysis, data cleaning and manipulation were performed. For methodology and queries, please refer to the repository.

* Happiness Report: 2,200 records (all countries from 2008-2022)
* World Bank Open Data: World Development Indicators Database 
   * Health dataset: 16,000 records
   * Government dataset: 7,000 records
   * Education dataset: 12,000 records
   * Environment dataset: 6,000 records
   * Economy dataset: 14,000 records 
* WHO data: dataUNODC database (Violent and Sexual Crime Dataset): 6,000 records


<img width="764" alt="Screen Shot 2024-10-03 at 7 29 44 PM" src="https://github.com/user-attachments/assets/d8e1ae77-aa93-4b0e-940a-ce8cca6b7cd3">


# Executive Summary

## Overview of Findings 

The most significant indicators influencing a country's overall happiness are health and education. The greatest relationship and predictive indiciator is access to basic healthcare, particularly clean drinking water and life expectancy. While numerous confounding factors affect a country's happiness, the following sections will explore additional impactful indicators and highlight key insights for happiness improvement opportunities. 

Below is an overview dashboard showcasing the average happiness scores and indicators from 2012 to 2022. The statistical relationship will be detailed throughout the report and the interactive dashboard can be accessed [here](https://public.tableau.com/views/WorldHappinessIndicatorMap/Map_dash?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link). 


<img width="1103" alt="Screen Shot 2024-10-04 at 4 11 03 PM" src="https://github.com/user-attachments/assets/8fa34a0b-063f-40c8-bc55-20a00fd09851">


### Indicator Trends 

* Over 50% of the indicators had a correlation greater than 0.8
* The strongest relationships with happiness scores are found in the health, education, and economy categories
* Regression analysis examines how much the happiness score is expected to change based on the indicator value
* The categories with the strongest effect on happiness are health, education, and economy
* The correlational analysis can be found in a supplementary dashboard [here](https://public.tableau.com/views/SupplementaryCorrelationandRegression/Supplement?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

  <img width="1018" alt="Screen Shot 2024-10-04 at 4 44 08 PM" src="https://github.com/user-attachments/assets/2fb14e26-e610-46fa-9cc3-b5a28d53a43e">


### Key Predictive Indicators 

* Indicators with statistical significance (p-value < 0.05) and a correlation greater than 0.8 are visualized below and can be accessed [here](https://public.tableau.com/views/HappinessCorrelationandRegression/Analysis_dash?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) 
* Health is the strongest predictive indicator for happiness, with universal healthcare and health expenditure showing a high correlation (> 0.8)
* The lower secondary education completion rate is another predictive indicator; however, the country’s expenditure on education is not significant and does not have a strong correlation
* This may be due to factors (such as poverty and lack of access to basic needs) that limit children's ability to complete lower secondary education, which helps explain the high predictive indicators of a country’s poverty rate and government effectiveness

<img width="1093" alt="Screen Shot 2024-10-04 at 4 46 31 PM" src="https://github.com/user-attachments/assets/53e6b2f0-88fb-4276-b0a0-f7dbb2a137cd">


### Recommendations 

* First recommendation: Increase government's effectiveness in health expenditure allocation for basic health care
* Second recommendation: Improve government spending allocation to address issues that limit children from completing lower secondary school (for example, addressing poverty)
* Recommended initiatives can include providing meals in lower secondary schools and increasing job oppourtunities in lower secondary school systems 

#### Next Steps 

* After the implementation of recommended initiatives, an analysis of government spending, government effectiveness, and happiness scores is highly recommended to further explore their effectiveness and impact.
* Other indicators to be further explored include population density and its effect on government effectiveness and spending.
* Some limitations of this analysis include the lack of information on environmental indicators, such as access to green spaces and safe living conditions. Further exploration of environmental indicators is highly recommended, given the significant effects of PM2.5 and CO2 emissions on happiness.
* Another limitation of the study is the lack of data provided by countries, resulting in NULL values. It is important to account for NULL values in the analysis. For example, violence rates and literacy rates were not reported in most of the 20 bottom-ranked countries, which may have affected its significance to the analysis. Additionally, some top and bottom-ranked countries did not report lower secondary completion rates for certain years. When dealing with large datasets across countries, it is essential to address this concern and design an analysis that can accommodate these issues.




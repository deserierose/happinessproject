# Happiness Project 

## Happiness Project 

### Abstract 

The disparity of happiness amongst countries has been well established by the World Happiness Report, founded in 2012. Their thorough investigation between confounding factors with happiness scores has provided valuable insight into economic and social trends around the world. However, the purpose of this analysis is to conduct a deeper investigation on additional indicators that may affect a country’s happiness and to provide a comprehensive view of the data from 2012 to 2022. This analysis provides an up to date summarization of happiness score trends and aims to provide targeted recommendations for policy makers, improving the quality of life within impoverished nations.


### Project Objective 

Identify key indicators that have the highest impact on a country's overall happiness
Identify trends between indicators and happiness scores
Provide recommendations for policy makers to improve the overall happiness of a country 


### Methods and Results 


#### Data Sources 

Happiness Report 
World Bank Open Data: World Development Indicators Database
WHO data: dataUNODC database (Violent and Sexual Crime Dataset)

##### Methods


Excel 
SQL 
Python 
Tableau 

 
For all datasets, data for all countries from 2012 to 2022 were collected (see repository for raw data). Each indicator dataset was pulled based on the data available and based on its relevance to four categories: education, government, environment, economy and health. Indicator datasets were not used in the analysis if most countries did not provide the data or if the dataset contained mostly null values. Each dataset underwent pre-processing in Excel for standardizing, addressing duplicates, trimming and dropping columns not relevant to analysis. Each dataset was then imported to PostgreSQL for analysis. SQL was used for further cleanup, general analysis (top/lowest countries, null values) and manipulation (transposing, averages, joining tables). For statistical analysis, countries were ranked by pulling the top 20 happiest countries and the top 20 unhappiest countries and assigned a country ID to be used as a primary key. All statistical analysis was done on ranking countries. Each indicator was also assigned to one of four categories: education, government, environment, economy and health. With SQL, correlational analysis was conducted on ranking countries comparing each indicator and their happiness scores from 2012 to 2022. With python, a regression analysis was then followed comparing happiness and each indicator within their category. Categories with the best fit and indicators with the greatest significance were then visualized for further analysis. Using SQL, the average of the happiness scores and the average of each indicator value was queried for visualization. For further processes and queries, see notebook listed in repository.

### Results 

For results, see correlation analysis and regression analysis in the repository.  

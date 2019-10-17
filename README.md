# Bias in Data

Name:Richard Todd

Date: 10/13/2019

## Goal
The goal of this project is to explore the causes and consequences of bias in datascience through an examination of data on Wikipedia articles. 

## Data sources used
This project uses three sources of data:

1) Data on English-language Wikipedia articles within the category "Category:Politicians by nationality" made available on figshare under the CC-BY-SA 4.0 license:
- https://figshare.com/articles/Untitled_Item/5513449 Politicians by Country from the English-language Wikipedia. figshare. Dataset. 

2) Population data from the United Nations International Indicators, made available under a CC BY 3.0 license. This data was provided in csv format as part of the class assignment, but is also available at the link below:

- https://www.prb.org/international/indicator/population/table/ 2018 World Population Data Sheet.

3) Output from the ORES ("Objective Revision Evaluation Service") machine learning package. In this data, each page is assigned one of six quality categories used in English Wikipedia content assessment, made available under a CC BY 3.0 license.

- https://en.wikipedia.org/wiki/Wikipedia:WikiProject_assessment#Grades

## Resources used
This analysis was prepared using Python 3.7 running in a Jupyter Notebook environment.  
Documentation for Python can be found here: https://docs.python.org/3.7/  
Documentation for Jupyter Notebook can be found here: http://jupyter-notebook.readthedocs.io/en/latest/  

The following Python packages were used and their documentation can be found at the accompanying links:
pandas
numpy
json
requests

## Files Created
This notebook creates 2 CSV files of data extracted and compiled as part of this analysis.
1) `wp_wpds_countries-no_match.csv` containing Wikipedia page records that do not match population data
2) `wp_wpds_politicians_by_country.csv` containing merged wikipedia pages and country-level population data

For ease, three CSV files of raw data are also included (see above).

## Data Tables Created
In the analysis section of the workbook, the below summary tables are created (see notebook for details):

* Top 10 countries by coverage: 10 highest-ranked countries by politician articles as a proportion of country population
* Bottom 10 countries by coverage: 10 lowest-ranked countries by politician articles as a proportion of country population
* Top 10 countries by relative quality: 10 highest-ranked countries by relative proportion of politician articles that are of GA and FA-quality
* Bottom 10 countries by relative quality: 10 lowest-ranked countries by relative proportion of politician articles that are of GA and FA-quality
* Geographic regions by coverage: Ranking of geographic regions (in descending order) in terms of the total count of politician articles from countries #### * Geographic regions by quality: Ranking of geographic regions (in descending order) in terms of the relative proportion of politician articles from countries in each region that are of GA and FA-quality FA-quality

## License

- This assignment code is released under the MIT license in `LICENSE.txt`.
- See above for data source licensing.
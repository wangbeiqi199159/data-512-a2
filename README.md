# Bias in Data

## Goal of the Project

This is an analysis of how the coverage of politicians on English-language Wikipedia and the quality of articles about politicians varies between countries. 

This project reflects the existence of bias in data analysis.

## License and Terms
[MIT License](https://opensource.org/licenses/MIT)

[CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

## Relevant Data Scource and API

**Article data:**The wikipedia dataset can be found on [Figshare](https://figshare.com/articles/Untitled_Item/5513449).

**Population data:**The population data is on the [Population Research Bureau website](http://www.prb.org/DataFinder/Topic/Rankings.aspx?ind=14). 

**ORES:** The article quality data is from [ORES ("Objective Revision Evaluation Service")](https://ores.wikimedia.org/v3/#!/scoring/get_v3_scores_context_revid_model).

## Data

### Source Data

Data from Figshare:

|  Column | Description |
|---| ---|
| country  | containing the sanitised country name, extracted from the category name|
|  page| containing the unsanitised page title. |
|  last_edit | containing the edit ID of the last edit to the page.|

Data from opulation Research Bureau website:

|  Column | Description |
|---| ---|
| Location  | country name|
|  Location type| country |
|  TimeFrame| Mid-2015|
|  Data Type| number|
|  Population| population|

Two files are stored under ```raw_data``` folder.

### Variables of Final Data File

Final data stores in ```cleaned_data.csv``` under folder ```cleaned_data```.

Variables shown as follows:

|  Column |
|---|
| country  |
|  article_name|
|  revision_id |
|  article_quality|
|  population |

## Data Process and Analysis

Prerequiste Packages:

- requests

- json 

- csv

- pandas

- numpy

- matplotlib.pyplot

There will be visualizations to show:

1. the countries with the greatest and least coverage of politicians on Wikipedia compared to their population.

2. the countries with the highest and lowest proportion of high quality articles about politicians.

```a2-bias-in-data.ipynb``` under ```scr``` folder contains all code and information of data processing and analysis.

## Directory Structure

```
data-512-a2 (master)
|
|     License
|     README.md
|	    
|----- raw_data
|     | 
|     |      page_data.csv
|     |      Population Mid-2015.csv
|     | 
|----- cleaned_data
|     |      
|     |      cleaned_data.csv
|     | 
|----- scr
|     |      
|     |      a2-bias-in-data.ipynb
|     | 
|----- visualizations
|     |      
|     |      10 Highest-ranked Country In Terms Of Articles Per Population (%)
|     |      10 Highest-ranked Country In Terms Of High-quality-article Rate (%)
|     |      10 Lowesr-ranked Country In Terms Of Articles Per Population (%)
|     |      10 Lowest-ranked Country In Terms Of High-quality-article Rate (%)

```




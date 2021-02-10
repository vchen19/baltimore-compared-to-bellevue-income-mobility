# baltimore-compared-to-bellevue-income-mobility

## Background and Introduction

Recent sociology research and elevated cries for social justice have shaken the country’s faith in the “American Dream,” with increasing evidence that a child’s destiny is extremely closely tied to the neighborhood and circumstances they grow up in. [Empirical and anecdotal evidence](https://www.nytimes.com/2015/05/04/upshot/an-atlas-of-upward-mobility-shows-paths-out-of-poverty.html) all point to the idea that it is unreasonable for policymakers to ask people to simply “pull themselves up by their bootstraps” to achieve success. Intergenerational [income has long been used as a method for measuring social mobility](https://www.econstor.eu/bitstream/10419/33437/1/514190388.pdf). The ability of a child to move from a lower income percentile to a higher one is a sign that a society sufficiently provides the resources for people to overcome hardships and achieve better lives, a core facet of the “American Dream.” 

The two cities in comparison in this study are Bellevue, WA and Baltimore, MD. Bellevue has been rated by [USA Today as the 2nd best place to live in the United States](https://www.usatoday.com/story/money/business/2014/09/17/24-7-wall-st-50-best-cities-to-live/15736533/). [Nearly 24% of Baltimore’s population lives below the poverty line](https://money.cnn.com/2015/04/29/news/economy/baltimore-economy/). 

## Business Question

How likely is it that a child whose parents come from the bottom 25% of income are able to advance an income quartile in Baltimore and in Bellevue? 

## Data Sources

Data was retrieved from [The Opportunity Atlas](https://www.opportunityatlas.org/), a data science project that uses Census data to evaluate various metrics of social mobility. [The specific dataset used for this analysis](https://github.com/vchen19/baltimore-compared-to-bellevue-income-mobility/blob/main/all_tract_household_income_low_parental_income.csv) consisted of average household income for those with low parental income (in the bottom 25%) for all Census tracts in the United States.

## Methods

Average household income data was found in every Census tract for low parental income (bottom 25%) by The Opportunity Atlas. The datasheet was sorted by tract and by city in order to isolate the tracts in Bellevue and in Baltimore. Using nested IF statements, the incomes of each tract were assigned to income quartiles and income percentiles in tens (10th percentile, 20th, etc.)  based on this data. The same procedure was performed on the entire dataset, for all tracts in the United States. Using COUNTIF statements, the number of tracts in each quartile and bracket were found for each city and for the entire dataset. The counts were turned into percentages of the total number of tracts within that city. The same procedure was performed on the entire dataset. These percentages of number of tracts that fell into buckets of tens of percentiles were plotted for Baltimore, Bellevue, and for the entire United States. 

## Results
![alt text](https://github.com/vchen19/baltimore-compared-to-bellevue-income-mobility/blob/main/income_distribution.png "Income Distribution")

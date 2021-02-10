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
![alt text](https://github.com/vchen19/baltimore-compared-to-bellevue-income-mobility/blob/main/income_distribution_table_quartiles.png "Table Income Distribution in Quartiles")

From the data, we can see that in all areas of Bellevue, children whose parents had income in the bottom 25th percentile make on average a quartile higher, since the average incomes for this group of people in those areas all fall in the 2nd quartile. In Baltimore, by contrast, this is only true for about 28% of the Census tracts, with 72% of Census tracts having an average income that is also in the bottom 25th percentile. 45.8% of all tracts in the United States are able to have average household incomes a quartile above their parents. A similarity between Baltimore and Bellevue is that neither had tracts with average household incomes above the 50% percentile. This is perhaps indicative of the power low parental income has on a child. Despite growing up in two vastly different cities, two children from similar economic backgrounds will not have drastically different fates.

## Analysis

These two examples are an interesting example of disparities in social mobility in cities. In Bellevue, it is likely that you will be able to make more than your parents, and in Baltimore, it is unlikely. This data indicates that factors outside of one’s control, such as the neighborhood one grew up in, can fairly significantly determine one’s socioeconomic destiny. This challenges our traditional beliefs around the American Dream and whether or not hard work and hard work alone is enough to improve your life.

These signs point to the fact that social mobility is much less likely in Baltimore than it is in Bellevue. This has interesting implications for institutional policy. Because education is a primary means of social advancement in this country, initiatives to improve education outcomes are necessary to improve social mobility. For example, the [Baltimore Scholars Program](https://apply.jhu.edu/baltimore-scholars-program/#:~:text=The%20Johns%20Hopkins%20University%20is,%24150%2C000%20and%20have%20typical%20assets.), gives generous tuition assistance to Baltimore City High School students that are accepted into Johns Hopkins, helping to facilitate social mobility through academic achievement. A program like this is much more necessary in Baltimore than it is in Bellevue, where no such program exists.



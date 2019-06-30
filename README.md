# Budweiser Data Analysis Report
__MSDS 6306 Case Study 01 Budweiser__
by: Christian Nava and Phillip Hale


![](https://images.askmen.com/1080x540/sports/fanatic/mystery-budweiser-super-bowl-ad-1102806-TwoByOne.jpg)


_note: this data, report and analysis is not indicitive, related or represent the Budweiser corporation or organization in any form and should be considered a fictional representation_


## Introduction
Anheuser-Busch, from Budweiser, requested the analysis of top data scientiest Christian Nava and Phillip Hale from SMU to provide insights into the various beer styles consumed in the United States. Budweiser has provided the following data sources: 
* [Beers](https://github.com/BivinSadler/MSDS-6306-Doing-Data-Science/blob/master/Unit%207/Beers.csv)
* [Breweries](https://github.com/BivinSadler/MSDS-6306-Doing-Data-Science/blob/master/Unit%207/Breweries.csv)

Please refer to [Appendix](https://github.com/naivelogic/MSDS-6306-Case-Study-01-Budweiser#appendix) for details _(e.g., data dictionary)_ on the above datasets. 



## Analysis
Please refer to the Rnotebook for detail analysis on findings. At a high level... 


<<<<<<< HEAD
#### One Way ANOVA
For further analysis for Budweiser, we suppose the CFO and busines manager have interest in monitoring the `ABV` _Alcohol by volume of the beer_ for each of the State (total of 51 states). For each state, we have collected the `ABV` per state and applied a one-way ANOVA to compare the State's ABV content. 

$$H_0: \mu_state1 = \mu_state2 = .... \mu_state51$$

$$H_a: Not all \mu_stateX, are equal or at least one is different from others$$
=======

### One Way ANOVA - ABV vs State Comparision
For further analysis for Budweiser, we suppose the CFO and busines manager have interest in monitoring the `ABV` _Alcohol by volume of the beer_ for each of the State (total of 51 states). For each state, we have collected the `ABV` per state and applied a one-way ANOVA to compare the State's ABV content. 

$H_0: \mu_state1 = \mu_state2 = .... \mu_state51$

$H_a: Not all \mu_stateX, are equal or at least one is different from others$
>>>>>>> 0a90c92f6d4908d30d893dc7050b13ace64f620a


Below is a plot of the `ABV` content by `State`:


<<<<<<< HEAD



=======
![](https://github.com/naivelogic/MSDS-6306-Case-Study-01-Budweiser/blob/master/data/Fig1%20for%20ABV%20v%20State.png)



### Histrogram (Graph 2) For EDA
>>>>>>> 0a90c92f6d4908d30d893dc7050b13ace64f620a
Below is a histogram of the IBU distribution of beer. 
![](https://github.com/naivelogic/MSDS-6306-Case-Study-01-Budweiser/blob/master/data/hist%20of%20IBU%20distribution.png)



## Appendix 
### Data Dictionary - Beer
__Name__ | __Definition__ 
--- | ---
Name| Name of the beer.
Beer_ID | Unique identifier of the beer.
ABV | Alcohol by volume of the beer.
IBU | International Bitterness Units of the beer.
Brewery_ID | Brewery id associated with the beer.
Style | Style of the beer.
Ounces | Ounces of beer.

### Data Dictionary - Breweries
__Name__ | __Definition__ 
--- | ---
Brew_ID | Unique identifier of the brewery.
Name | Name of the brewery.
City | City where the brewery is located.
State | U.S. State where the brewery is located.

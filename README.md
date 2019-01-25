# Video_Games_Sales
This report explores a dataset generated by a scrape of vgchartz.com. The scraping script is available at https://github.com/GregorUT/vgchartzScrape. The dataset contains video games sales and attributes for approximately 11493 video games. The dataset contains 16,598 observations and 11 variables.


## Data


There are 16,598 observations about 11493 video games, with 11 features, as descrived below.
**Variables Dictionary:**
* Rank - Ranking of overall sales
* Name - The games name
* Platform - Platform of the games release (i.e. PC,PS4, etc.)
* Year - Year of the game's release
* Genre - Genre of the game
* Publisher - Publisher of the game
* NA_Sales - Sales in North America (in millions)
* EU_Sales - Sales in Europe (in millions)
* JP_Sales - Sales in Japan (in millions)
* Other_Sales - Sales in the rest of the world (in millions)
* Global_Sales - Total worldwide sales.


## Univariate Analysis

* The main features in the data set are Global_Sales and Year, and discovering the trend around them, i.e. what are the top globally selling value of the other features, and top other features values over time.
* The month of the year could likely contribute to the rise of sales. For example, certain video game genres could be always popular in a certain month of the year. It would be interesting to see how the other regions around the world's sales do, rather than just having the variable Other_Sales. Lastly, demographic data on the buyers of these games could tell us a lot on why certain feature values happen to be more popular than others. In fact, such kind of data can also help us predict the future sales considering the buyers demographic and behaviour.
* In order to create the regional sales comparison plots in the **Multivariate** section, I needed to combine the regional sales columns (NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales) by using the gather function from the tidyr package.
* I had to drop observations where the Year had an N/A value.


## Bivariate Analysis

* 2008 and 2009 were the most successful years for the game community. Action games are more famous nowadays. Nintendo and PS2 are behind the highest global sales. The top globally selling video game since 1980 is Wii Sports.
* The strongest relationship you found is one explained in the correlation matrix in the regional sales section.


## Multivariate Analysis

* Although the action genre was the popular famous since 2000, the second popular genre Sports (as we saw in the bivariat analysis) peaked in 2006. This was further confirmed after plotting A. the globally selling games per year and finding out it was Wii Sports from the Sports genre in 2006, and B. the globally selling games per genre, and C. the globally selling games platform which of course is Wii.
* The global and regional yearly sales for North America and Europe further confirm the results found in the correlation matrix, where the plots show that a rise in each of these regions whenever the global sales rises. On another note, the globally selling per year plots for publishers and platforms show an interesting pattern, where for example between 2006 and 2009 the Nintendo publisher was dominant, and the Wii platform was dominant. This makes sense since Nintendo owns Wii, and was released for the first time in November 19, 2006. Video game publishers that also happen to own platforms/consoles publish a couple of games that work with their new product to help market it. Other publishers follow to ensure a competitor's advantage.


## Reflection

* Since 1980, video games global sales reached a total of 8920.44 million.
* Action games have been the most popular for over a decade. They contribute to almost 20% of the games released.
* Play Station is the most popular platform.
* Wii Sports is the top video game by revenue.
* Namco Bandai Company is producing maximum number of successful games.
* There is huge spike in the number of releases after 2000 and it peaked during 2008 and 2009.
* 2009 was the most successful year for the video games community.
* The last 5-6 years has seen a decrease in the revenue.
* EA is the top most publisher by number of releases.
* DS is the top most platform by number of releases.
* Wii Sports in 2006 generated huge revenue compared to all other games along the years.
* Nintendo has been dominating the market as the top publisher by revenue in 24 years since 1980.
* Releasing too many video games does not garantee more sales as we have seen in the case of Nintendo, Sony Computer Entertainment and Ubisoft, where they were in the top selling publishers list but not in the top releasing publishers list.
* Once a platform clicks in the market i.e. top selling, it goes on to rule for few years (3-6 years).
* North America and Europe contribute 75% of the market share by revenue, and both had their sales peak in 2006, although the global sales peak was in 2008.

[Video_Games_Sales.html](): A full report on the insights found.

One aspect that limited this analysis is the absence of the sales of other parts of the world, rather than just having the variable Other_Sales. Also, the month of the year could likely contribute to the rise of sales. For example, certain video game genres could be always popular in a certain month of the year. For future work, I would like to find data on the buyers demographic which could explain a lot of the resons behind the trends found, and improve the analysis. It will also help draw recommendations to the decision makers in this industry on where to focus their budget; which genre, which region, which platform, etc.

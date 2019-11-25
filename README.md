# Education In Africa

Investing in young minds as a business model.

# Abstract
The *African Development Bank Group* statistical data portal offers an immense range of socio-economic indicators for each African country from 1960 until now. This three-dimensional data precision (country, year, over 200 indicators) provides sufficient tools for our project to perform a spatio-temporal analysis of the educational factors in African countries and the impact on their social and economical growth. 

The African continent is made of young developing countries and is full of unexploited resources and unexplored richness. This thus provides a ground for development and growth. In an absence of financial resources and historical power, education is the best tool for a socio-economical revolution, especially when we consider that this continent has a demographically young population. 

As a further endeavor, using machine learning tools, we hope to come up with a new socio-economic index quantifying the effectiveness and importance of a country's efforts in developing education.


# Research questions
* What are the general trends of education importance in African countries in relation to georgraphy and time?
* What relations can be extracted between education and other socio-economic indicators?
* What conclusions can be drawn from the importance of education in economic growth?
* What factors are most influenced by the educational approach of each country?
* Can we come up with a new index measuring the effectiveness of the educational endeavours of each country?

# Dataset
The datasets we will use are retreived from the *African Development Bank Group* statistical data portal. A series of 200+ socio-economic indicators are provided for each country, per year. Each entry of the datasets is for a specific indicator, for a specific country and for a specific year. A grouping will be performed based on the countries, years and indicators such that the cleaned dataframe would be using a two-dimensional indexing: **country** & **year**. The columns will then correspond to the different indicator values.
* [AfDB Socio Economic Database, 1960-2019.](https://data.humdata.org/dataset/afdb-socio-economic-database-1960-2019)
* [Fragile States - Socio Economic Database, 2015.](https://data.humdata.org/dataset/fragile-states-socio-economic-database-2015)

The datasets would eventually be complemented with further data if needed.

# A list of internal milestones up until project milestone 2
Our dataset is quite imposant with nearly 2.8 Million row information, because of the multiple indexes we have, since 1960, for every single country in the African continent.
We didn't have any missing value to deal with for most important columns (Date,country..), missing values were in the indexes values.

## 1.Education
We first extracted all Education-related indexes by looking for Education keywords in the names and descriptions of all our indexes.
We went further by reading their descriptions (They were only 28) to be sure that indeed they are education indexes.
One example would be eliminating some GDP index because it had "international" in its description, when we were looking for "intern" or "internship" with prefix "intern".
Finally, we eliminated highly correlated attributes (> 0.95), we kept the significant ones, which were 6 at the end.
With that done, we manipulated our data each time to get the information we needed for each task, for instance we looked deeper into our final six attributes(indexes) by plotting them and analysing what we've observed for the whole continent(AFR) in all possible years(where information is available).
We also produced maps to see the differences in each of the indexes values for each Country, in one specific year.

## 2.Socio-Economical Growth
Extracting compelling social & economical indicators:
We looked at the key economical indicators for development on several online resources. The most commonly used were the following:
* Human development index (HDI)
* Unemployment rate
* GDP per capita
* Inflation
* Corruption
* Gender Inequality
* Poverty
* Income Inequality
Although the dataset contains values for the previously mentionned fields, some included a considerable number of missing fields as some countries did not give statistics about them. We looked for the indicators in the dataset that had a wide enough range of values. 

## 3.Next 
* We will perfom a detailed geographical analysis on the distribution of our indicators (both education and development) using the visual maps generated.
* A more thorough analysis of the meaningfullness of the kept socio-economic indicators is required for the next milestone before correlating them with the education indicators found and hence try to find an index measuring the effectiveness of education and its contribution to the socio-economical growth.
* We want to find a formula summarizing education in only one index. We will try to use machine learning tools for this operation.
* We will interpret the influence of education on countries' growth and depending on the observed results, we will eventually compare the education domain to others (agrictulture, service... ) and if it's really "worth it" to invest in one or the other. 
* We will eventually try to come up with a way to create a X,Y relationship for a linear regression model representing the impact of education on economical development. Feature selection tools will be used in an extensive manner.
* For the comparison part, we will restrain the year range to between 1980 and 2015 as most of the values for the indicators are missing outside of this time period. 

# Questions for TAa


# Obesity in America 

## Factors and Trends of Obesity 

 

### Authors: Kendall Lipsey, Kayla Kirk, Tanner Miles

 

## Introduction: 

Obesity is defined as being over 20% of your body’s ideal weight1. In clinical settings, body mass indexes (BMI) measure body fat and are used to determine obesity and overweight classifications2. 

Nearly 40% of the overall United States population, roughly 100 million people, is considered to be obese3. Seven individual states report an obesity rate of 35% or higher within their population4.  Obesity is linked to over 60 chronic diseases5. Many factors influence whether a person is likely to be obese, and these may include race, gender, ethnicity, income and education level. Obesity can increase the risk for heart disease, stroke, diabetes, some cancers, and many other major health issues. In turn, this can cost Americans $147 billion per year in medical expenses6. 

## Methodology:  

### Data Collection 

Datasets were collected from the Center for Disease Control’s, or CDC’s, website. The CDC conducts the Behavioral Risk Factor Surveillance System to monitor obesity and overweight status of US citizens in all 50 states and US territories7. The Behavioral Risk Factor Surveillance System also evaluates the obesity and overweight status among various demographic, income, educational attainment, age, and gender groups.  Separately, the CDC collects data on rates of breastfeeding mothers among various groups as well8 . Both datasets were downloaded from the CDC’s website as comma-separated-values.  

Further data was collected to evaluate a wider scope of obesity over time. This dataset was available as a comma-separated-values document and downloaded9.  

Data Importation and manipulation 

Pandas was imported into Python III using the interactive computing environment JupyterHub. Pandas was used to read in both datasets and convert them into Pandas Dataframes. The format provided of the obesity data was cumbersome to extract usable information. The data was transformed into usable columns for a handful of manipulations; however, complex Booleans were primarily used to extract data for analysis. For example, 9 distinct booleans were applied to the dataframe to extract data on obesity levels for age groups (See Appendix, Figure 1). 

Data was extracted on the following parameters: gender, income level, age group, race, obesity, overweight, educational attainment, breastfeeding status, state, and year. Larger scale analysis was done for the average for the entire US population (rather than a state-by-state analysis).  

### Data Visualization 

Bar charts illustrated percent obesity over the years 2011-2016, percent overweight over the years 2011-2016, percent obesity among age groups (18-24, 25-34, 35-44, 45-54, 55-64, and 64 and older), percent obesity among the highest and lowest ranked US states,  income among the highest and lowest ranked US states, and percent obesity among racial groups (non-Hispanic white, non-Hispanic Black, Asian, Native American, 2 or more races, White, and Hawaiian/Pacific Islander) (See Appendix, Figures 2, 3, 4, 10, 11, 12, 18 ). Age groups and racial groups were predetermined in the datasets. Matplotlib was imported and utilized to make both vertical and horizontal bar graphs. A user-defined-function was applied to the bar chart illustrating obesity among age groups to display the obesity rate directly above each bar. 

Grouped bar charts were used to illustrate the percent of obesity for years 2011 to 2016 among income brackets(<$15,000, $15,000-$25,000, $25,000-$35,000, $35,000-$50,000, $50,000-$75,000, and over $75,000), genders (male and female), and educational attainment levels (less than high school, high school, technical school, and college degree) (See Appendix, Figures 13, 5, 14 ). These levels/brackets were predetermined in the datasets. To create the grouped bar charts, Matplotlib was imported and utilized. Furthermore, a grouped bar chart was used to compare the percent overweight and percent obese over the years 2011 to 2016. Numpy was utilized in many of the graphs to create arrays of ranges for specifying vertical and horizontal axes. To avoid overlapping in visualizations, a ‘width’ was applied to the x-axis argument of grouped bar charts.  

Line charts were used to illustrate obesity rates over time (1975 to 2016), obesity rates among age groups for the years 2011-2016, and obesity and breastfeed rates among US states (See Appendix, Figures 21, 9, 17). The line plots utilized matplotlib and seaborne. Additionally, NumPy was used to create arrays of ranges for specifying vertical and horizontal axes. 

To create a scatter plot of the top and bottom five most obese states for males and females on a US map, cartopy, matplotlib (pyplot) were used (See Appendix, Figures 7, 8). Cartopy’s NaturalEarthFeatures for land, coastline, and borders were used with longtidue formatter and latitude formatter. This process was repeated for Hawaii for more fluid visualizations. Matlotlib was further used to make a pie chart of the percentage of male and female obese in the year 2016 (See Appendix, Figure 6). 

Plotly was also used to illustrate a map of the United states, shading states corresponding to their respective obesity rates and breastfeeding rates (See Appendix, Figures 15, 16). No regressions or correlation coefficients were determined as they were out of the scope of the course subject matter. 

 

## Results:  

### Obesity over Time (generational): 

For the years 1975 to 2016, the average rate (among all US states) of obesity was evaluated. Although there were miniscule variations, the obesity rate was found to rise consistently over the time period investigated (See Appendix, Figure 21). In 1975 the obesity rate was just under 12% which rose steadily to 20% in 1993, and 30% in 2007.  

### Obesity over Time (2011 to 2016): 

For the years 2011 to 2016, the average rate (among all US states) of obesity was evaluated (See Appendix, Figure 2). Although there were miniscule variations, the obesity rate was found to rise consistently over the time period investigated. In 2011 the obesity rate was just over 27% which rose to nearly 30% in 2016. 

### Overweight over Time: 

For the years 2011 to 2016, the average rate (among all US states) of overweight was evaluated (See Appendix, Figure 3). Although there were miniscule variations, the overweight rate was found to decrease consistently over the time period investigated. In 2011 the nearly 36% of the population was overweight which decreased to just over 35% in 2016. This decrease in magnitude was less than the accompanying increase in obesity during the same time period.  

### Gender: 

For the years 2011 to 2016, the average obesity rate (among all US states) was evaluated for both males and females (See Appendix, Figure 5). For both genders, obesity rates increased consistently each year during this time period. Although it was found that males had higher obesity rates every year except 2013 (were the obesity rate for males and females was equal), the difference is within a fraction of a percent and is negligible (See Appendix, Figure 6). When compared geographically (the highest and lowest obesity states for males and females), most states were overlapping as a top 5 for both males and females (See Appendix, Figures 7, 8). For those which were only in the top five fore males or females, if you included the top 10 states, overlap was again shown. Notably, Hawaii had some of the lowest rates for female obesity and Colorado had the some of the lowest rates for both male and female obesity.  

### Age Groups: 

For the years 2011 to 2016, the average obesity rate (among all US states) was evaluated for the following age groups: 18-24, 25-34, 35-44, 45-54, 55-64, and 64 and older. For every age group, the obesity rate consistently increased over the time period (See Appendix, Figure 9). The 18-24 year olds were found to have the lowest obesity rates among the age groups every year from 2011 to 2016, with an obesity rate of only 17.3% in 2016 (See Appendix, Figure 10). The 25-34 year olds had the second lowest obesity rates in 2016 with only 27.2% obese. However, this was not always the case. In 2013, the 64+ year olds started having higher obesity rates than the 25-34 year olds, and in 2016 the 64+ year olds had 28% obesity. In 2016, 35-44 year olds had an obesity rate of 33.1%, ranking the third most obese age group. They have maintained this ranking for all years in timeframe. In 2016, 55-64 year olds had an obesity rate of 34.2%. Although this age group had been ranked highest obesity rates all years prior, they dropped to number two in 2015. Lastly, in 2016 the age group with the highest obesity rate of 35.1 were the 45-54 year olds. 

### Income: 

For the years 2011 to 2016, the average obesity rate (among all US states) was evaluated for the following income brackets: <$15,000, $15,000-$25,000, $25,000-$35,000, $35,000-$50,000,  $50,000-$75,000, and over $75,000.  Those with the highest rate of obesity are included in the lowest income bracket (See Appendix, Figure 13). Those who attain an income of less than $15,000 per year and between $15,000 and $25,000 report an obesity rate of over 30%. When entering the $25k-$35k income bracket, we see an obesity rate of less than 30% for the years 2011-2013, however, the rate increases to above 30% beginning in 2014. This trend is similar for the next two levels of income. When achieving an income of greater than $75,000 per year, the obesity rates drop significantly. The previous bracket, $50k-$75k, hovers around 28% to 30% over the six-year span, but the rate for $75k+ averages near 23% topping out at 25% for 2016. These results show a negative correlation between income and the rate of obesity. As income increases, the rate of obesity decreases. Similarly, there is a very drastic difference between those achieving a low yearly income versus those achieving a high income. Notably, West Virginia had both the lowest income and highest obesity for males and females.  

### Educational Attainment: 

For the years 2011 to 2016, the average obesity rate (among all US states) was evaluated for the following levels of educational attainment: less than high school, high school, some college or technical school, and college degree (See Appendix, Figure 14). Those who have achieved less than a high school education report the greatest obesity rate. For all years, the obesity rate for this category is above 30%, averaging near 33%. Though the obesity rate is steadily increasing for all educational categories, there is an obvious decrease in the rate as you receive more education. Those who have received a high school diploma as well as individuals with some college or technical school education, report an average obesity rate near 30-31%. However, when we move into the category of college graduate, the rate drops significantly. This category is still increasing over the six-year time frame, though it is minimal. The average rate of obesity among those with a college degree is near 21-22%. A negative relationship also exists within this variable-as education attainment increases, the rate of obesity decreases. 

### Race: 

The average obesity rate (among all US states) in the year 2016 was examined for the following racial groups: non-Hispanic white, non-Hispanic Black, Asian, Native American, 2 or more races, White, and Hawaiian/Pacific Islander, and other (See Appendix, Figure 18).  Obesity rates among the races varied, with non-Hispanic Black with the top obesity rate of 38.3% followed closely by Native American with an obesity rate of 38.1%. At 33.1%, Hispanic had the third highest obesity rate followed by individuals of 2 or more races at 31%. Hawaiian/Pacific Islander had obesity rates of 30.6%, while White was 28.3%. Other races averaged at 26.1% obesity while the Asian obesity rate dropped dramatically to 9.8% which is the lowest rate. As these racial categories are nominal with no ordinal properties, only observational associations can be made. 

### Breastfeeding: 

When evaluated at a state level, no association was found between breastfeeding and obesity rates (See Appendix, Figures 15, 16, 17). In a handful of cases, the obesity appeared inversely relational to breastfeeding rates. However, this observation was not consistent enough for further investigation.  

## Discussion: 

In the years 2011 to 2016, the rate of obesity increases while the rate of overweight decreases. A correlation is suggested here that some of the overweight individuals are entering the obese category rather than entering the normal category. Future studies are suggested to evaluate this association.  

Hawaii ranks in the five lowest obesity rates for females, while Colorado ranks in the five lowest obesity rates for both males and females. Additionally, Hawaiian/Pacific Islanders are ranked as 4th lowest obesity among the 9 racial groups investigated. Both Colorado and Hawaii have some of the most progressive health care policies in the United States. Future studies are suggested to investigate if health care policies are related to obesity rates. 

We are interested in learning more about the relationship between variables in our data set. Does income and age interact to create a greater obesity rate? Similarly, what is the relationship between race and age? We know that as age increases, the obesity rate steadily rises, and falls after age 64, but does this hold true across all races individually.  As mentioned before, those who attain a higher income report a lower rate of obesity, but we also need to consider the cost of living in states we are focusing on. The cost of living is higher in Colorado as opposed to West Virginia, and those states report the lowest and highest obesity rate in the country. That relationship may be worth exploring. To go along with that, we are interested in policies that state governments are implementing to combat obesity and the costs and risks that come with it. Different healthcare options may exist for those living in, again, Colorado and West Virginia.   

 

 

 

 

 

 

 

 

 

 

# Obesity and Food Access in North Carolina 

 

## Introduction: 

Access to food is not evenly distributed throughout North Carolina. Worse, low access to food is disproportionately concentrated for people with low income. This results in More than 2 million people in North Carolina, including over 435,000 children under the age of 15, live in areas where residents are suffering with diet-related disease and can’t easily access healthy food.10 North Carolina’s varied population density offers more insight into this issue. People who live in rural areas are at higher risk of obesity, have lower access to healthy foods, and eat fewer fruits and vegetables than their urban counterparts.11 These factors combined warrant investigation on a geographic basis of North Carolina, obesity rates, and access to food.  

## Methodology: 

### Data Collection 

For the North Carolina food access data analysis, Datasets were collected from the US Department of Agriculture (USDA) Department of Economic Research Service.12 The USDA’s ‘food atlas’ is a collaborative research database of various access levels to fresh and affordable foods, on a county level, for the entire United States. This dataset was available as a Microsoft Excel table which was downloaded and converted to a comma-separated-values document. Additionally, a data set was collected from the Robert Wood Johnson Foundation13 to observe the obesity rates in every county in North Carolina. This dataset was also available as a Microsoft Excel table which was downloaded and converted to a comma-separated-values document. 

### Data Importation and Manipulation 

Pandas was imported into Python III using the interactive computing environment JupyterHub. Pandas was used to read in both datasets and convert them into Pandas Dataframes. Columns were renamed to increase readability and the two dataframes were merged into one dataframe. The data was narrowed to only evaluate North Carolina and data was extracted on the following parameters: percent of the population with low access to a store, percent of the population with low income and low access to a store, percent of households with no car and low access to a store, obesity, county, and year. 

### Data Visualization 

Plotly was utilized to illustrate a map of North Carolina counties and their corresponding obesity levels and food accessibility (See Appendix, Figure 19,20). 

 

## Results: 

There appeared to be an association between obesity and the percent of the population with low income and low access to a store in North Carolina counties (See Appendix, Figures 19, 20). Observations included the highest obesity rate in North Carolina was found in Halifax County (and similar rates in the surrounding counties). Similarly, these counties were rated some of the highest for percent of the population with low income and low access to a food store. Moreover, Coastal communities had, on average, lower obesity paired with lower percentage of the population with low access to food stores. 

## Discussion: 

In North Carolina, the association between low access to food stores and obesity is of much interest. Local food drives and community support, in addition to subsidies and policy, are of interest. Future work is suggested to investigate the relationship between such policies and local obesity. 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 Project-1: The Effect of COVID on Crime in the City of Los Angeles

### Objective
The goal of this project was to determine the potential effects of the Covid-19 pandemic on crime in the city of Los Angeles
Research Questions:
1.	Was overall crime lower during the Covid-19 pandemic?
2.	Did crime shift by bureau over time?
3.	Did the pandemic affect the number of victims by gender?
4.	Was there was an increase in domestic violence and child abuse?

Methodology:
Data Set: City of LA Crime Dataset 2010 – 2019 and 2020-Present
Analyzed data in two stages: 
Stage One: Focused on the total number crimes reported, crimes reported in different areas
Stage Two: Focused on the race and/or ethnicity of the victims, a subset of the type of crime reported, and the gender of the victims
Hypothesis and Null Hypothesis:
Null Hypothesis
•	Overall Crime: Covid-19 did not have a significant effect on crime in Los Angeles
•	By Bureau: Covid-19 did not have a significant effect on crime in each area of Los Angeles
•	By Gender: Covid-19 did not have a significant effect on the victim gender
•	By Type: Covid-19 did not have a significant effect on domestic violence and child abuse

Alternate Hypothesis
•	Overall Crime: Covid-19 did have a significant effect on crime in Los Angeles
•	By Bureau: Covid-19 did have a significant effect on crime in each area of Los Angeles
•	By Gender: Covid-19 did have a significant effect on the victim gender
•	By Type: Covid-19 did have a significant effect on domestic violence and child abuse


### Annual Crime Summary 

#### This analysis comprised of multiple steps:
  - Created a new dataframe the total number of crimes indexed by the year
  - Percentage Change per year was calculated and added to the new dataframe
  - A Summary Statistics table was generated
  - IQR, upper and lower bounds were calculated to confirm that there were no outliers
  - Created an Annual Crime Summary dataframe consisting of the most common occurring data from each of our columns indexed by year
  - Plotted a bar graph of the Total Crimes by Year (with the mean visible)
  - Plotted a line graph of the Percentage Change by Year
  - Plotted a linear regression of the Total Crimes by Year
  - Ran a T-Test of Pre-Covid and Covid-Era Yearly Total Crimes by slicing the data.  

![](./output_data/TotalCrimeYTY.png) 


![](./output_data/PercentChangeYTY.png)


![](./output_data/LinearRegressionYTY.png)


#### Results:
  - There were no statistical outliers in the Annual Total Crimes data
  - Three out of the Four Covid-Era years were below the mean of the entire 14 year period in the dataset
  - The Percentage Change analysis showed that very similar decreases in total crime occurred in 2014 and 2020
  - The linear regression produced an r-value of 0.0095, showing a weak linear relationship of total crimes over the years
  - The Annual Crime Summary showed that with further research, Hispanic Victim Data and Single Family Dwellings have the potential to be key indicators in grasping the total crime in Los Angeles
  - The T-Test calculated a p-value of 0.2469, which shows that, while the Covid-Era mean was 155124 compared to Pre-Covid mean of 170625 the difference between the Covid-Era and Pre-Covid means do not have a statisically significant difference between them



### Area Summary

1.  We selected all of the different Areas .
2. Placed all areas in four bins: Central, South, West, Valley. 
3. Pre Covid Data
   a: filter your DataFrame to include only the data for the years 2010 to 2019 and grouped by Area Name and Crime Year.
   b: Then group it by Area Name and calcuate the mean.  
4. Covid Data 
   a: Did same thing with data for 2020 to 2023  

5. Plotted a Bar Graph               

![](./output_data/Crime%20Per%20Area.png)

6. Using the geoapify API made the maps for Hot Spots for Pre Covid Data and Covid Data

[https://api.geoapify.com/v2/places](https://api.geoapify.com/v2/places)

![](./output_data/Pre_covid.png)
![](./output_data/covid_era.png)  

7. Merged the data of Area Name/ Pre Covid Years/ Mean Data and Area Name/ Covid Years/ Mean Data

8.Used Chi Square to calculate the p value#Merged the data of Area Name/ Pre Covid Years/ Mean Data and Area Name/ Covid Years/ Mean Data 

### Null Hypothesis : There is no statiscal difference between two datas
### Hypothesis: There is a statiscally significant difference.

                        Types of Crimes Gender Summary
 Counted all of the unique values in 'Types of Crime' column                     
#find all the unique values in 'Types of Crime' column
Defined different categories
 Listed all crime descriptions
 Categorize each crime description
Plotted a pie Chart

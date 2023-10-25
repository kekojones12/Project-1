# Project-1
The Effect of COVID on Crime in the City of Los Angeles

The goal of this project was to determine the potential effects of the Covid-19 pandemic on crime in the city of Los Angeles
Research Questions:
1. 	Was overall crime lower during the Covid-19 pandemic?
2. 	Did crime shift by bureau over time?
3.	   Did the pandemic affect the number of victims by gender?
4.	   Was there was an increase in domestic violence and child abuse?

Methodology:
Our analysis sources two datasets of every crime incident from the Los Angeles Police Department, from 2010-2019 and 2020-2023, respectively.
These records were transcribed from handwritten and typed police reports, and have the potential for inaccuracies
Our assumption for this project was that the Covid-19 era took place from the 2020-2023
After collecting and concatenating the datasets into one comprehensive dataframe, the columns were reduced to the information that helped 

Hypothesis and Null Hypothesis:

Null Hypothesis
Overall Crime: Covid-19 did not have a significant effect on crime in Los Angeles
By Bureau: Covid-19 did not have a significant effect on crime in each area of Los Angeles
By Gender: Covid-19 did not have a significant effect on the victim gender
By Type: Covid-19 did not have a significant effect on domestic violence and child abuse

Alternate Hypothesis
Overall Crime: Covid-19 did have a significant effect on crime in Los Angeles
By Bureau: Covid-19 did have a significant effect on crime in each area of Los Angeles
By Gender: Covid-19 did have a significant effect on the victim gender
By Type: Covid-19 did have a significant effect on domestic violence and child abuse


                           Crime Summary 

Created a Summary Statistics table of the total crimes over the entire dataset
Bar plot of the total crime count over the length of the dataset
   

![](./output_data/TotalCrimeYTY.png)
Line graph showing the percentage change in total crimes year-to-year

Linear Regression plot

T-Test of Pre-Covid and Post-Covid Yearly Total Crimes by slicing the data.






                    Area Summary

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

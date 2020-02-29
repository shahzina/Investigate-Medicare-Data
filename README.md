# Investigate Medicare Dataset from 2014

This project explores and analyses health data from 2014 focussing on the home health agencies that provide medicare services. The dataset provides us information about the providers such as their names and geographical locations but it also describes patient-related data like, LUPA and non-LUPA beneficiaries, categorizing patients according to their race and diseases, etc..The datasets were procured from kaggle and then cleaned and downloaded from there using google BigQuery, all other cleaning and wrangling was done in a jupyter notebook.  

Pandas, numpy, matplotlib, seaborn, uszipcode library, scipy and gmaps are the tools used to analyze the data. The file "Project 1- code" has the code used for data exploration and visualization and the file "Project 1- essay" has the explanation and inferences from the resulting data, charts and graphs. 

The following image shows the distribution of agencies across the country and the agencies with no latitude and longitude is shown in the second figure:
![agencies](https://github.com/shahzina/Investigate-Medicare-Data/blob/master/images/agencies_by_state.png)

![N/A_agencies](https://github.com/shahzina/Investigate-Medicare-Data/blob/master/images/agencies_with_null_locs.png)

The following histograms show a distribution of all diseases, 
![disease_hist](https://github.com/shahzina/Investigate-Medicare-Data/blob/master/images/disease_column_histogram.png)

### Patient percentage by disease- <br> 
The ailments that the patients were diagnosed with are divided into 16 categories which have been stored by agency in our dataset. The following is a pie-chart showing the distribution.
![disease](https://github.com/shahzina/Investigate-Medicare-Data/blob/master/images/patients_by_disease.png)

### Patient by race- <br> 
There are 5 races that have been identified and the remaining have been clubbed into a sixth called 'other unknown beneficiaries'. The 5 beneficiaries are white, black, hispanic, pacific islanders and native american or alaskan native beneficiaries.
![race](https://github.com/shahzina/Investigate-Medicare-Data/blob/master/images/patients_by_race.png)
 
 
The following heatmap shows the distribution and concentration of agencies in the US. Due to missing data, some areas seem completely devoid of an agency. 
![heatmap](https://github.com/shahzina/Investigate-Medicare-Data/blob/master/images/map.png)


### Results of Regression Analysis - <br>
1- Slope of line is negative implying a negative relationship between both variables. <br>
2- r value is also negative. <br>
3- slope of line is -10.56.  <br>
4- standard error is 0.56. <br>

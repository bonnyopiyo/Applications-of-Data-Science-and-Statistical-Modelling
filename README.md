# Applications-of-Data-Science-and-Statistical-Modelling
# Analysis on Traffic Accidents in the UK
## Objectives
Download the csv file “accidents2019.csv” data https://data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-safety-data.

The data was originally downloaded from the UK Department of Transport Road Safety data
base (“Road Safety Data - Accidents 2019”)

You can read further information about the data is in the website.

# The analysis covers the following areas with some questions of interest in each.

## General
1. How many accidents happened in 2019?
2. What are the column names in the data frame?
3. Report the date (day/month/year) and coordinates (longitude and latitude) of the accident in the
100th row of the data frame. (The row at the top of the data frame counts as the 1st row.)
4. Columns containing information about the type of vehicles involved in the accident.

## Casualties
1. The total number of casualties.
2. The difference in the number of casualties between Lower Layer Super Output area (LSOA)
E01032739 (City of London 001F) and E01033708 (Hackney 027G).
3. The LSOA that saw the highest total number of casualties in 2019.

## Police officer attendance
1. What are the possible values that occur in the column Did_Police_Officer_Attend_Scene_of_Accident,
and how often does each value occur?
2. The value Did_Police_Officer_Attend_Scene_of_Accident = 1 indicates that a police officer
attended the accident. What do the other value(s) in that column mean? (Consult the data web
site to answer this question.)
3. What fraction of accidents was attended by a police officer?
4. What fraction of those accidents that happened on a weekday was attended by a police officer?
How does this number compare to the corresponding fraction for accidents on weekends?

## Visualisation
1. Visualise the locations of all accidents by a scatter plot of Latitude vs Longitude. Annotate the
axes, add a plot title, and increase the figure size to 10in by 10in.
2. Create a similar scatter plot as in the previous question 1. but zoom in on a 2 by 2 degree area
that includes Exeter/Devon, and choose a different color for accidents that happened in a rural
area and in an urban area. Include a red marker that indicates the coordinates of Exeter/Devon
(as per wikipedia).
3. Are accidents at higher speed limits more likely to be fatal than at lower speed limits? Answer the
question with an appropriate data visualisation and a short written summary.

## Regression analysis
To complete the following questions, you have to load the “Linnerud physical exercises data” from the
scikit-learn package using the following commands:

  from sklearn.datasets import load_linnerud
  
  linnerud = load_linnerud()
  
  ### Questions
1. State the author’s last name and year of the study in which that data first appeared.
2. Using the appropriate function from the scikit-learn package, fit a simple linear regression model
with number of chinups (Chins) as the target variable, and “Weight” as the covariate. Report the
fitted regression coefficients, and interpret the slope coefficient.
3. Your lecturer is a middle-aged male, 170 pounds (“Weight”), 32 inch waist size (“Waist”), and a
resting heart rate of 70 (“Pulse”)? How many chin-ups (“Chins”) do you think he can do? (Use
linear regression in scikit-learn on the Linnerud data to answer the question.)


## Dimensionality reduction
1. What linear combination αwW +αcC +αpP of the physiological variables weight W, waist circumference C and pulse P has the highest possible variance among all possible linear transformations?
State the weights αw, αc and αp rounded to 2 decimal places. (The variance maximisation is
subject to the constraint α
2
w + α
2
c + α
2
p = 1 and you may assume that the appropriate scikit-learn
function adheres to this constraint.)
2.  What might the interpretation of this one-dimensional representation of a person’s physiological
factors be, and in what context could it be useful?
3. What is the variance of the linear combination with αw = αc = αp =
q
1
3
and how does this
variance compare to the variance of the linear combination calculated in question 1 in this section?


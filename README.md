# gun-violence-usa
Analysis of gun violence incidents and state legislation between 2014-2017

![Untitled presentation (1)](https://github.com/juliewhitton/gun-violence-usa/assets/84740189/da7cc1ef-3d72-4fcd-b9b8-05925b4d1247)

# Project Introduction
I chose this project as the culminating achievement in order to complete my Data Immersion course at CareerFoundry. I am passionate about the state of gun violence in this country, legislation, and, of course, data. I will continue to work on this project indefinitely as I have many unanswered questions. 
As it stands, I have conducted an analysis investigating the rate of gun violence incidents by state, the strength of each state's gun laws, and which political party governed each state's legislative party by year. 

# Data and Sources
I sourced and compiled 4 different data sets in order to conduct this analysis. My main source was this data set from Kaggle:
https://www.kaggle.com/datasets/jameslko/gun-violence-data. James scraped the data from gunviolencearchive.org. The following is from James' data citation:

From the organization's description:
Gun Violence Archive (GVA) is a not for profit corporation formed in 2013 to provide free online public access to accurate information about gun-related violence in the United States. GVA will collect and check for accuracy, comprehensive information about gun-related violence in the U.S. and then post and disseminate it online.

I then found a data set regarding gun laws by state and year from:
[https://www.icpsr.umich.edu/](https://www.icpsr.umich.edu/web/ICPSR/studies/37363). While not entirely comprehensive, it includes 134 firearm safety laws and indicates whether or not it is in place in each state by year. I analyzed the variable descriptions and created 15 gun safety categories on which to base my analysis.

Here is the official citation from ICPSR:

Citation:
Siegel, Michael. State Firearm Law Database: State Firearm Laws, 1991-2019. Inter-university Consortium for Political and Social Research [distributor], 2020-02-26. https://doi.org/10.3886/ICPSR37363.v1
Funding: United States Department of Justice. Office of Justice Programs. National Institute of Justice (2016-MU-MU-0047)

In order to calculate and normalize the rate of incidents I needed population data for each state and year. The data I used can be found here: https://www2.census.gov/programs-surveys/popest/tables/2010-2019/state/totals/nst-est2019-01.xlsx
Citation:

Table 1 Annual Estimates of the Resident Population for the United States, Regions, States, and Puerto Rico: April 1, 2010 to July 1, 2019 (NST-EST2019-01)
Source: US Census Bureau, Population Division
Release Date: December 2019

I then needed the ruling party of each state's legislative branch by year and found PDF files here:

https://www.ncsl.org/about-state-legislatures/state-partisan-composition

I loaded the PDF files into Excel, retrieved the necessary data and converted it to a csv file.

# Tools Used

### Python

LIBRARIES:

pandas\
numpy\
seaborn\
matplotlib\
matplotlib.pyplot\
os\
sklearn\
&nbsp;&nbsp;&nbsp;&nbsp;from sklearn import preprocessing\
&nbsp;&nbsp;&nbsp;&nbsp;from sklearn.cluster import KMeans\
&nbsp;&nbsp;&nbsp;&nbsp;from sklearn.preprocessing import StandardScaler\
pylab\
&nbsp;&nbsp;&nbsp;&nbsp;from pylab import rcParams\
statsmodels.api\
&nbsp;&nbsp;&nbsp;&nbsp;from statsmodels.tsa.stattools import adfuller\
&nbsp;&nbsp;&nbsp;&nbsp;from statsmodels.graphics.tsaplots import plot_acf, plot_pacf

### Folium GIS

### Excel

### Tableau

Here is the link to my Tableau storyboard:
https://public.tableau.com/app/profile/julie.whitton/viz/GunsandPoliticsintheUnitedStates/GunsandPolitics.

### Usage

Please feel free to use any of the data in my repo and/or code from my notebooks. Please note that there are several notebooks containing assigned tasks utilizing K clustering, (Un)supervised ML, Time Series analysis, etc that are included in the repo but are not relevant to the project.


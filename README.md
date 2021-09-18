# Uber-NYC-Data
Analyzing the number of Uber pickups in New York City based on the weather conditions

## Intorduction:

Weather Forecasting is a blessing to the humans, as the smooth operation of a variety of businesses depends on the weather conditions.
One such domain is Transport. Transportation is strongly affected by weather conditions
Be it planning of whether to travel from one place to another or price surge in cab rates or the public transport facilities; all depend on weather forecasting for their smooth functioning.
Adverse weather conditions can cause disturbances for all means of transport. During winters, low temperatures and snowfall or fog can result in road traffic, accidents and jams as well as delays or cancellations of trains or flights.
Analysis of the trends observed in different modes of transport can help the concerned Transport Departments in better planning for prevention of mishaps.

## Dataset

The Dataset being used in the project is: uber_nyc_enriched.csv
The source of the dataset is Kaggle.
The dataset consists of 12 columns and 29102 rows.

The dataset provides details about the various Boroughs from which cabs were taken, the weather conditions described by features like Wind Speed, Visibility, Temperature, Dewpoint, Sea Level Pressure, Precipitation in the last 1 hr, 6 hrs and 24 hrs, Snow Depth and whether it is a holiday or not.

The target is the number of pickups based on all these weather conditions.

## Pre-processing

The dataset needs to be preprocessed so that no erroneous results are obtained.
Steps followed for preprocessing of uber_nyc_enriched.csv dataset:
Data Cleaning
       - The dataset was checked for any Null (nan) values 
          and rows containing null values were removed from
          the dataset
       - The dataset was checked for any duplicate row entries 
          and the duplicate rows were dropped 
 2.   Encoding
        This step was performed to convert labels into 
        machine-readable numeric form
        Method used: Label Encoding

Followed by these steps a Heatmap depicting the correlation between the various features was plotted 
And this was followed by splitting the data into train and test.
70:30 ratio was used for train:test respectively

## Algorithms

- Clustering
  The data was modeled for clustering using sklearn
  Method used: K-Means Clustering

- Regressors
The following regressors were used:
1. Decision Tree Regressor
2. Random Forest Regressor
3. Ensemble

Accuracy Score:
Decision Tree Regressor: 64.7%
Random Forest Regressor: 79.8%
Ensemble: 77%

## Conclusion
Random Forest Regressor gives us the highest accuracy score.
Though the scores of other regressors are close enough, Random Forest Regressor proves to be the best in this case.
Clustering gives us an idea about the number of pickups each borough witnessed out of the 5 boroughs that have been taken under study here.






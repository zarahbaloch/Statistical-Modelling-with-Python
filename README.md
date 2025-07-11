# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal of this project was to explore and model the relationship between bike availability and surrounding points of interest (POIs) using real-world API data. By connecting to the CityBikes, Foursquare, and Yelp APIs, I aimed to understand whether specific features could predict the number of available bikes at different stations.

## Process
### Step 1 
Connected to the CityBikes API to retrieve real-time bike station data
### Step 2
For each station, I used Yelp and Foursquare APIs to collect POI data (i.e restaurants, bars, review counts, and average ratings)
### Step 3
Cleaned and merged everything into a single dataset with one row per station.
### Step 4
Built a regression model using statsmodels to see if those POI features had any real relationship with the number of free bikes.
### Step 5
Interpreted the model results 

## Results
- The regression model had a low R-squared (~0.026), so POI features alone didn’t explain much of the variation in bike availability.
- None of the predictors were statistically significant, so no strong conclusions could be drawn about their influence.
- Yelp offered more detailed POI data (e.g., ratings and reviews), while Foursquare had broader location coverage.
- A classification-based approach (e.g., labeling stations as having “low”, “medium”, or “high” availability) might be more useful than regression in this context.
  

## Challenges 
- Inconsistent API responses and missing data required extra cleaning and grouping logic.
- Merging data from Yelp and Foursquare was tricky due to differences in structure and available attributes.

## Future Goals
- Reframe the problem as a classification task, predicting bike availability levels instead of exact counts.
- Beyond the scope of the project, I think an interesting addition would be to develop a dashboard to visualize real-time station availability alongside predicted trends
- Integrate other data types which may have more direct influence on bike avaliability (e.g., time of day, weather conditions) to capture real-world bike demand dynamics.



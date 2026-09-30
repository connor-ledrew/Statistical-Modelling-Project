# Final Project: Statistical Modelling with Python

## Project/Goals
To demonstrate an understanding of API usage, environment variables, JSON-formatted data, EDA, data cleaning, SQLite in Python, and multivariate analysis.

## Process
1. Understand citybik.es
2. API request for Vancouver
3. Parse JSON response for various bike stations (241)
4. Compare Yelp & FourSquare data
    Yelp data restricted to points of interest within 3-square city blocks with a less-than-or-equal-to a 3 out of 4 price rating; limit 50 results.  The data was retrieved 2023-02-27 around ~9pm PST, however the data was timestamped at 2023-02-13 @ 7:22pm (monday).
5. Join the city_bike data with the yelp dataset
6. EDA
7. Replicate joined data in SQLite
8. Backward elimination multivariate linear regression

## Results
No statistically significant relationship was found between Vancouver's points of interest (Yelp reviewed) and total bike share slots. It was postulated that additional bike slots would be allocated for areas with more popular businesses. However, analysis of the discovered variables show that there is little evidence to support this claim. Subsequently, it appears the typical city bike user is not primarily interested in points of interest.


## Challenges 
1. Difficult to see a valuable overlap between a snapshot of bike share usage in a city and points of interest.  bike share data has a lot of noise from regular users who likely are commuting to non-POI (such as work or friend's houses).
2. The FourSquare categories were inconsistent, according to their documentation this is to maintain legacy categories.  Likely need more advanced methodologies to wrangle the data. 


## Future Goals
A more valuable analysis could be conducted if additional time was allocated to:
1. Collecting usage data over time
2. Understanding the typical bike-share user behaviour to predict where to build/decommission stations and/or restock bikes.
3. Look for statistically significant relationship between bike-share usage and major chains, which may sponsor additional infrastructure.

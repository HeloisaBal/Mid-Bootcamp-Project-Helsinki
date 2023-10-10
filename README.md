# Mid-Bootcamp-Project-Helsinki
### Purpose
This project is a descriptive analysis of the Helsinki City Bikes system in Finland.

### Source data
https://www.kaggle.com/datasets/geometrein/helsinki-city-bikes - > 10 million trips made between 2016-2020.
https://en.ilmatieteenlaitos.fi/open-data  - Meteorological data from 2016-2020.

### Documentation
Notebook - Helsinki City Bikes.ipynb reads both CSVs and draws insights from the data.
Presentation Results - Helsinki City Bikes.pdf contains data visuals summarising the insights.

### Summary
Converted both CSV files into usable pandas dataframes.
Performed data cleaning and wrangling on both datasets. In this step, I decided to drop 2016 and 2017 due to lack of trip data compared to the remaining years in order to have an even comparison.

After cleaning, I merged both datasets. On the merged, clean dataset, I used MinMaxScaler and OneHotEncoder to build a simple linear regression model to predict biking distances.
I also attempted to predict the day of the week when bike trips would take place, by using a multinomial logistic regression, however with just a 25% accuracy, which ended up not being useful.

#### Further areas to study would be:
- Building different models for different variables
- Predicting bike flow per dock for staffing purposes
  
In both cases, I would need more data.

### Conclusions drawn
- In Helsinki, the city bikes are mostly used for commuting purposes.
- The most popular biking hours are during the evening.
- The biking speed is considerably lower during weekends compared to weekdays.
- The bikes are not used for long trips, but for short ones.


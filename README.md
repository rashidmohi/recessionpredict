# USA Recession Predictor 
### A Simple Logistic Regression Solution built with the publicly available US Economic Data 
*Dec 2022*
### Please visit the following blog post for more details
https://medium.com/@mohiuddin.rashid/is-a-recession-coming-in-2023-43ce841be3e2

## Motivation
With the economic uncertainty at the end of 2022, people are anxious about the economic outlook for 2023 and if there is a recession on the horizon. In this analysis, I am attempting to answer the following questions
1. How well we can build the recession predictor with the publicly available data?
2. What are the key factors to predict recession?
3. What is the prediction for recession in 2023 using the selected models?

## Solution Approach
#### a) Data Preparation
1. Load data & clean date field
2. Prepare quarterly datasets
3. Prepare monthly datasets
4. Create the monthly merged dataset with 6-mth adv predictor field as target varible
5. Create the quarterly merged dataset with 2-qtr adv predictor field as target varible
6. Create the monthy and quarterly datasets with "%age change" variables and remove nulls

#### b) Model Development
7. Create the clean monthly and quarterly datasets for model fitting
8. Build the Logistic regression models on monthly and quarterly datasets for recession prediction
9. Analyze the metrics for the models and answer Q1
10. Analyze the model coefficients and answer Q2

#### c) 2023 Predictions
11. Load the 2022 datasets, generate 2023 predictions and answer Q3

## Datasets

| Dataset | Source |
| ------ | ------ |
| Recession | https://fred.stlouisfed.org/ |
| Gross Domestic Product (GDP) | https://fred.stlouisfed.org/ |
| Consumer Price Index (CPI) | https://fred.stlouisfed.org/ |
| Gold Future Price | https://www.investing.com/ |
| Unemployment Rate | https://fred.stlouisfed.org/ |
| Federal Funds Rate (Interest Rate) | https://fred.stlouisfed.org/ |
| Dow Jones Index (DJI) | https://www.investing.com/ |
| Housing Price Index (HPI) | https://fred.stlouisfed.org/ |

## Files

1. USA_Recession_Predictor.ipynb [The jupyter notebook]
2. .\data [folder for the training data]
3. .\pred_data [folder for the input data for prediction]

## How to Setup and Use this Model

1. Clone the project folder on your machine
2. Install the required packages from below (check the notebook for details)
* Numpy
* Pandas
* Scikit Learn
* Matplotlib
3. Run the notebook to train the models and generate metrics
4. For the prediction you can use the sample for 2022 OR create your own for another period


## License

MIT


## Author and Acknowledgements
Rashid Mohiuddin 
https://www.linkedin.com/in/rashidmohiuddin/

*Thanks to Udacity team for the inspiration, ideas and resources!*








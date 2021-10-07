# Used BMWs: Predicting Cost of Vehicles

## Project Description
 - This purpose of this project is to create a Regression model that predicts the cost of a used bmw in a dataset from kaggle.com
 - Project created using the data science pipeline (Acquisition, Preparation, Exploration, Analysis & Statistical Testing, and finally Modeling and Evaluation)

## Project Goals
 - Create a Final Jupyter Notebook that reads like a report and follows the data science pipeline
 - In the Jupyter Notebook Create a regression model that performs bettern than our baseline mean RMSE and R-squared scores
 - Create Function Files to help peers execute project reproduction
 - Create a baseline Machine Learning Model that creates a baseline for easy and equal car pricing predictions

  ## Deliverables
 - Final Jupyter Notebook
 - Function Files for reproduction
 - Detailed Readme

  ## Executive Summary
 - The purpose of this notebook is create a regression model that predicts the price of used bmw vehicles in a dataset from kaggle.com
 - Target variable: price
 - Best features determined: 
    - year
    - mileage
    - tax
    - mpg
    - engineSize
    - is_diesel
    - is_hybrid
    - is_manual
    - is_semiauto
    - is_automatic
 - In conclusion, the end result and real world application is provide a baseline for bmw dealerships to work together to create equal pricing in their vehicles for a more satisfied customer base.
 - RMSE:  5121.33
 - R-squared:  0.80

 ## Hypothesis
 - Mileage driven and year the vehicle was manufactured are going to be the highest predictors in predicting price of the vehicles

 ## Findings & Takeaways
 - The features that I hypothesized (mileage and year) had the strongest correlation in relation to our target variable (price)
 - The Polynomial Regression Model with 2 degrees 
 - Our model performed extremely well and outperformed the baseline.
 - With more time I'd like to use feature engineering to help make the model more accurate in predicting vehicle prices

  # The Pipeline

 ## Planninng

 With some domain knowledge I want to test some regression models using the features hypothesized above: vehicle mileage and year manufactured. It is my belief that these will have the strongest correlation with our target: price

 ### Features Used in Modeling

 These features were used in modeling after being selected by the recursive feature elimination function within the scipy library

 - year
 - mileage
 - tax
 - mpg
 - engineSize
 - is_diesel
 - is_hybrid
 - is_manual
 - is_semiauto
 - is_automatic

 ### Model Performance
 - Using the mean for baseline and not the median

| Model                            | RMSE Train Score | RMSE Validate Score | R-squared |
|----------------------------------|------------------|---------------------|-----------|
| Baseline Mean                    | 11380.64         | 11537.31            | 0         |
| LinearRegression                 | 6425.741         | 7003.348            | 0.6315    |
| LassoLars                        | 6428.416         | 6993.942            | 0.6325    |
| TweedieRegressor                 | 8103.085         | 8522.972            | 0.4542    |
| PolynomialRegression (2 degrees) | 4649.406         | 6355.770            | 0.6965    |

### Test on Polynomial Regression: 2 Degrees
 - RMSE:  5121.33
 - R-squared:  0.80

  ### This is better than our baseline

 ## Project Recreation
 - Use the functions in the .py files and follow the pipeline flow of the notebook
 - Link to dataset: https://www.kaggle.com/mysarahmadbhat/bmw-used-car-listing



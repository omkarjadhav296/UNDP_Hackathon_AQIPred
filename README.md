# AQI Predictive Modelling

This repository contains the code and resources for the AQI Predictive Modelling project. The main objective of this project is to predict the Air Quality Index (AQI) using various machine learning techniques.

## Introduction

Population density, industrial activity, agricultural practices, thermal power plants, energy sectors, automotive industries, and transportation all affect air pollution differently (Ravindra, 2019; Ravindra et al., 2020). Aside from harming the ecosystem, air pollution also has negative effects on human health, including premature death, skin rashes, lung infections, respiratory tract infections, pneumonia, lung cancer, and heart failure (Manisalidis et al., 2020). Several important factors determine air pollution in a given area, including particulate matter, gaseous pollutants, and meteorological factors, necessitating AQI estimation by a large number of government and non-government organizations worldwide (Bao & Zhang, 2020; Li et al., 2020).
Among others, Particulate Matter 2.5 (PM2.5), Particulate Matter 10 (PM10), Carbon Dioxide (CO2), Carbon Monoxide (CO), and Nitrous Oxide (NO2) are key contributors to AQI. An increased AQI due to these substances negatively impacts the environment in numerous ways, including global warming, acid rain, the development of smog and aerosols, decreased visibility, and climate change (Balakrishnan et al., 2019).
Based on information from 2010 to 2019, the World Health Organization (WHO) published a report on global air quality in 2022. This study examined a wide range of air pollutants and discovered that PM2.5 was rising globally based on studies of 6,743 cities in 117 different nations, causing 1.7 million yearly mortalities in India alone. The top 20 cities with the highest air pollution included 18 Indian cities, illustrating the seriousness of India’s air pollution and adverse health effects in the years to come (Gurjar et al., 2016; Guttikunda et al., 2014).
A high AQI number denotes the most hazardous environment for people, posing significant health risks. Consequently, AQI monitoring and forecasting have become crucial tools for sustainable development (Rybarczyk & Zalakeviciute, 2021). Various researchers have created AQI prediction models based on statistical, deterministic, physics-based, machine learning, and deep learning techniques. However, the rigidity of traditional statistical and decision-making models makes them unsuitable for dealing with complex, nonlinear processes associated with air pollution.
Recent sensor developments have made it easier to identify different air pollution levels, allowing for automatic AQI calculations. With readily available datasets, AQI forecasting has become more straightforward (Bekkar et al., 2021). Machine learning techniques offer high precision and consistently predict AQI under all environmental conditions. The growing availability of historical air quality data allows machine learning models to produce more accurate forecasts, establishing them as viable alternatives to traditional statistical models for time-series forecasting. Given the complex, nonlinear nature of pollutant concentrations and their interactions, machine learning models provide an effective means of AQI prediction by identifying correlations between independent variables.


## Methodology

### `st_01_PredModel.ipynb`

This Jupyter Notebook contains the implementation of the predictive model for AQI. The notebook includes the following sections:

1. **Data Loading and Preprocessing**: This section covers the steps to load the dataset and preprocess it for modeling. It includes handling missing values, feature engineering, and data normalization.

2. **Exploratory Data Analysis (EDA)**: In this section, various visualizations and statistical analyses are performed to understand the distribution and relationships within the data.

3. **Model Building**: This section includes the implementation of different machine learning models such as Linear Regression, Decision Trees, Random Forest, and Gradient Boosting. Each model is trained and evaluated using appropriate metrics.

4. **Model Evaluation**: The performance of each model is evaluated using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²). The results are compared to determine the best-performing model.

5. **Results and Conclusion**: This section summarizes the results obtained from the models and provides insights into the predictive performance.

## Results

The results obtained from the `st_01_PredModel.ipynb` notebook are as follows: Based on the evaluation, the Gradient Boosting model was selected as the best-performing model for AQI prediction.

### **GBoost Model Results Explanation**

The results obtained for the GBoost model are as follows:

- **Score on train data: 0.9985721056938172**
  - This indicates that the model explains approximately 99.86% of the variance in the training data. The model fits the training data very well, suggesting a high level of accuracy on the training set.

- **Score on test data: 0.9879905328839844**
  - This indicates that the model explains approximately 98.80% of the variance in the test data. The model generalizes well to unseen data, maintaining a high level of accuracy on the test set.

- **Best parameters found:**
  - `n_estimators`: 200
  - `min_samples_split`: 7
  - `min_samples_leaf`: 2
  - `max_features`: 'auto'
  - `max_depth`: 5
  - `learning_rate`: 0.2
  - These parameters were identified as the optimal settings for the model through hyperparameter tuning, likely using techniques such as GridSearchCV or RandomizedSearchCV. They help in achieving the best performance by balancing the bias-variance trade-off.

- **Root Mean Squared Error: 0.10057397103366973**
  - This is a measure of the average magnitude of the errors between the predicted and actual values. A lower RMSE indicates better model performance. In this case, the RMSE is quite low, suggesting that the model's predictions are close to the actual values.

- **Overall model accuracy: 0.9879905328839844**
  - This is the same as the score on the test data, indicating the proportion of the variance in the dependent variable that is predictable from the independent variables. An accuracy of 98.80% is very high, indicating that the model performs exceptionally well.

In summary, the GBoost model demonstrates excellent performance with high accuracy on both the training and test datasets, low RMSE, and optimal hyperparameters that contribute to its effectiveness.


## Conclusion

The AQI Predictive Modelling project successfully implemented and evaluated various machine learning models to predict the Air Quality Index. The Gradient Boosting model was identified as the most accurate and reliable model for this task. Future work may include further tuning of the models and exploring additional features to improve predictive performance.

## Authors

- Er. Omkar Jadhav
- Er. Akshay Chaprana

## Acknowledgements

- Special thanks to the UNDP Hackathon organizers for providing the opportunity to work on this project.

# Bike_Sharing_Demand

This repository holds an attempt to predict bike sharing system demand using data from "Bike Sharing Demand" Kaggle challenge https://www.kaggle.com/competitions/bike-sharing-demand.

The task is to use machine learning to predict when will demand on bike sharing/renting system will increase/decrease by using past data.

The approach in this repository formulates the problem as regression task with series of features as input. Performance of 3 machine learning model compared.

My best model was random forest regressor.

Data
  Data: bike rent information
  Type: categorical and numerical
  Input: CSV file with features(windspeed, temperature etc) output: datatime + count
  Size: 1.22MB
  Instances: train (10887) and test (6494)

Preprocessing / Clean up
  -filling null values
  -checking for outliers
  -"datatime" feature separatin
  -dropping "casual" and "registered" from train dataset
  
Data Visualization
  - count vs other features scatterplot
  - correlation heatmap
  - predicted bike rental count over time
  
Problem Formulation
  Predict bike rent count by date based on season, temparature, humidty etc of that day.
  
  Models
    - Random Forest Regression Model
    - XGBoost Regression Model
    - LightGBM Regressor Model
   
Performance Comparison
   Mean Squared Error (MSE)
   R-squared (R2) score
   
   1 - Random Forest
   <img width="227" alt="Screenshot 2023-05-05 113031" src="https://user-images.githubusercontent.com/92418510/236515314-9fd4f752-6856-4b6d-a17d-d389430b462e.png">
   
   2 - XGBoost
   <img width="213" alt="Screenshot 2023-05-05 113318" src="https://user-images.githubusercontent.com/92418510/236515514-48a417a7-a855-4018-840d-883388ff3b1b.png">
   
   3 - LightGBM
   <img width="240" alt="Screenshot 2023-05-05 113414" src="https://user-images.githubusercontent.com/92418510/236515752-4e198d09-aaf2-4c3f-9ddf-7be4bb99d614.png">

    -------------------------------------------------------------------------

  Conclusions
  
<img width="334" alt="Screenshot 2023-05-05 112913" src="https://user-images.githubusercontent.com/92418510/236514802-46794c13-8673-4e78-934f-d9a0b2dab607.png">

  

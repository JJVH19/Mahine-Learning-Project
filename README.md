# Final Project

## Objective
The goal for this project is that I wanted to be able to classify each price for each car within a certain price range based on 8 bins of data and with features such as net worth, annual salary, age, and credit card debt.

## Dataset
For this analysis, I used the car_purchase dataset, https://www.kaggle.com/datasets/nileshthonte/car-price-prediction-with-ann. The dataset contains the data that I will categorize. Although it contains columns such as customer name, customer email, country, and gender, the focus of this dataset will be the age, annual salary, credit card debt, net worth, and car purchase amount.

## Data Exploration and Insights
- During the exploration phase, I observed a correlation between the prices of a car and the annual salary of the person buying the car.
  
![258611003-60ec744c-7f3e-4882-8dba-32a9ed318b56](https://github.com/JJVH19/Mahine-Learning-Project/assets/109435368/5c5dfb25-e163-4b9c-a181-f54db20f75a0)

- As shown below, people tend to buy a car based on their annual salary. Although this seems logical, it is a nice detail to take note of since it is a visualization of how the categorization would fit alongside the other features previously mentioned.
  
![258611005-33523ce4-a970-4f65-ad0e-6cbe48d7e8bd](https://github.com/JJVH19/Mahine-Learning-Project/assets/109435368/840dc9a8-ff2b-40ce-a20f-02826b5d13fa)


## Data Preprocessing
To ensure data quality and suitability for modeling, I performed the following preprocessing steps:
- Check for any outliers within the data and remove them
- Verified the data type
- Addressed missing data
- Scaled the data to avoid any bias

## Feature Selection/Engineering
I conducted feature selection/engineering to improve model performance. The selected features were:
- Annual salary
- Credit card debt
- Net worth
- Age

## Model Selection
After analyzing different algorithms, I chose the K-Nearest Neighbors (KNN) and the Random Forest algorithms as they are well-suited for this task. The reason being;
-  These models can handle the categorization I need for this project since I want to find a range within a certain price amount for a car.

## Model Training and Evaluation
The dataset was split into training and testing sets. I assessed their performances by tuning the hyperparameters of each model to select the best model. 
- The models were assessed based on their accuracy and F1_score metrics, producing the following results:
  - KNN Model: Accuracy and F1_score of 62%
  - Random Forest Model: Accuracy and F1_score of 58%

## Results and Conclusion
Based on the evaluation, I feel that I was able to create an effective classifier that will determine a car's price based on the features previously mentioned, using the KNN model.

## Future Recommendations
- For future work, I recommend a more in-detail tuning of the model's hyperparameters to further enhance the model's performance and achieve even better results.

## Limitations
It is essential to acknowledge the limitations of our approach and the dataset. In my case, a limitation would include the amount of data available from the dataset.

## Acknowledgments
I would like to express my gratitude to my instructor, Enfa Rose Geroge, and our TA, Bennett Brixen, for helping me have a better understanding of how to create this model.

## References
- https://stackabuse.com/k-nearest-neighbors-algorithm-in-python-and-scikit-learn/
- https://stackabuse.com/get-feature-importances-for-random-forests-with-python-and-scikit-learn/
- https://www.geeksforgeeks.org/random-forest-hyperparameter-tuning-in-python/#

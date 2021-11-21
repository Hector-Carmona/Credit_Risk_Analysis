# Credit_Risk_Analysis
Module 17 Challenge - Credit Risk Analysis

## Overview of the analysis

Apply machine learning to solve "Cedit Card Risk". Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, employing different techniques to train and evaluate models with unbalanced classes. 

We'll describe the balanced accuracy scores and the precision and recall scores of all six machine learning models.

## Results

### Random Oversampling

``` - Description: Instances of the minority class are randomly selected and added to the training set until the majority and minority classes are balanced.```

![Random Oversampling - Balanced Accuracy Score](https://user-images.githubusercontent.com/86028032/142768986-edab59c9-fce0-4aca-b354-c3f2e3340f2b.PNG)

![Random Oversampling - Confusion Matrix](https://user-images.githubusercontent.com/86028032/142768999-b0870c61-09e9-4537-9f4e-d24e4770e61e.PNG)

![Random Oversampling - Imbalanced Classification Report](https://user-images.githubusercontent.com/86028032/142769005-cf2b7b77-c2c4-4dbb-ae36-94fc3ef4678c.PNG)

#### SMOTE Oversampling

``` - Description: The size of the minority is increased by new instances being interpolated. That is, for an instance from the minority class, a number of its closest neighbors is chosen.```

![Smote Oversampling - Balanced Accuracy Score](https://user-images.githubusercontent.com/86028032/142769040-bf0f49bc-102f-4f34-902d-20450a1a34ad.PNG)

![Smote Oversampling - Confusion Matrix](https://user-images.githubusercontent.com/86028032/142769054-6e37aeba-ed33-4f7a-9280-65e290f8c669.PNG)

![Smote Oversampling - Imbalanced Classification Report](https://user-images.githubusercontent.com/86028032/142769058-8ecf8cb1-88c7-4105-bb90-550055a50f4b.PNG)

### Cluster Centroids Undersampling

``` - Description: Clusters of the majority class are identified, then generates synthetic data points, called centroids, that are representative of the clusters. The majority class is then undersampled down to the size of the minority class.```

![Cluster Centroids Undersampling - Balanced Accuracy Score](https://user-images.githubusercontent.com/86028032/142769117-8fc5daff-4483-460a-b261-df7854c008da.PNG)

![Cluster Centroids Undersampling - Confusion Matrix](https://user-images.githubusercontent.com/86028032/142769124-81766e58-b659-436d-ac0c-ac61b1f52aeb.PNG)

![Cluster Centroids Undersampling - Imbalanced Classification Report](https://user-images.githubusercontent.com/86028032/142769128-aa7a85f3-edc1-4ffb-88a5-9a0ebc0efe11.PNG)

### SMOTEENN Combination Sampling

``` - Descriiption: Combines the SMOTE and Edited Nearest Neighbors (ENN) algorithms.```

![Smoteenn Combination Sample - Balanced Accuracy Score](https://user-images.githubusercontent.com/86028032/142769154-5e0ed6cc-bea1-4a6b-aedb-bad30e6455df.PNG)

![Smoteenn Combination Sampling - Confusion Matrix](https://user-images.githubusercontent.com/86028032/142769152-ad2217b5-e3a0-40c2-961f-d7c1cac565a7.PNG)

![Smoteenn Combination Sampling - Imbalanced Classification Report](https://user-images.githubusercontent.com/86028032/142769153-5576a425-b7f1-4caa-9360-c934c119592a.PNG)

### Balanced Random Forest Classifier

``` - Description: The data will be sampled and then it's build several smaller samples, simpler decision trees. Each tree is simpler because it is built from a random subset of features.```

![Balanced Random Forest - Accuracy Score](https://user-images.githubusercontent.com/86028032/142769235-3e62145b-36dc-4310-b8e0-a7528b6d0bfe.PNG)

![Balanced Random Forest - Confusion Matrix](https://user-images.githubusercontent.com/86028032/142769236-748e93a8-aed4-4627-8819-fed365cb2a17.PNG)

![Balanced Random Forest - Imbalanced Classification Report](https://user-images.githubusercontent.com/86028032/142769233-cde9ded6-d706-4d9d-b502-52f0221b8cf6.PNG)

### Easy Ensemble Classifier

``` - Description: It involves creating balanced samples of the training dataset by selecting all examples from the minority class and a subset from the majority class. ```

![Easy Ensemble AdaBoost - Accuracy Score](https://user-images.githubusercontent.com/86028032/142769281-a3a522fd-39bb-4584-980a-4dd349c3f024.PNG)

![Easy Ensemble AdaBoost Classifier - Confusion Matrix](https://user-images.githubusercontent.com/86028032/142769278-727e558f-d032-4016-ab08-f3c8ccd0b0a8.PNG)

![Easy Ensemble Adaboost Accuracy - Imbalanced Classification Report](https://user-images.githubusercontent.com/86028032/142769282-b8516fff-77ed-454e-a213-2054f6fab97a.PNG)


## Summary

Easy Ensemble model records reveal to accurately identify and predict high risk loan applications.

The machine learning models that have been performed reveal the risk loan applications, so it is important to note their F1 score because it is average of the true positive rate (recall) and precision, where the best score is 1.0 and the worst is 0.0.


# Project Title:  SpicyCloud
That’s a spicy cloud: A comparative study to approaches for Tropical Storm intensity estimation from Raw and Infrared Satellite images using CNN

---

## Introduction:

- Tropical cyclones, which originate over tropical oceans, have become a topic of great concern due to their devastating impact on human populations. The intensity of these cyclones is primarily determined by the initial intensity of the cyclone and the wind speed.
- The records indicate a concerning 13-15% increase in the intensity of these cyclones since the late 1970s, underscoring the urgent need for advanced models to better comprehend and forecast tropical cyclone intensity. 
- Our project utilized a dataset comprising wind speed annotations and single-band satellite images obtained from over 600 storms, which was curated by the NASA IMPACT team in collaboration with the Radiant Earth Foundation. 
- Our research show that VGG-16 surpasses the other two conventional models (LeNet-5 and AlexNet) for the given task.

## Project Aim:
Creating an optimized CNN model with an in class regressor and comparing it to the VGG16 implementation for a tropical cyclone classifier with wind speed regressor.


## Final Model Description:

1. Convolutional Neural Network (CNN) architecture with three sets of Convolutional layers, BatchNormalization layers, and MaxPooling layers followed by two dense layers. 
2. Fewer layers than VGG16 without the VGG16's fully connected layers.
3. The model is optimized using the Adam optimizer and trained to minimize the categorical cross-entropy loss.
4. Our model was fine tuned to run as a regressor and a classifier.


## Experiments:

1. Running a base model regressor to compare the model RMSE with actual wind speed values.
2. Splitting the wind speed into 6 classes based on literature survey.
3. Using a VGG16 inference model and a recreated model to classify the dataset.
4. Optimizing Spicy Cloud to run as classifier based on appropriate error metrics and hyperparameter tuning.
5. Optimizing Spicy Cloud to run as a in class regressor after classification.

---

## Final Implementation:

![Base Model Vs Spicy Cloud Prediction](https://github.com/Shubhkirti24/SpicyCloud/blob/main/Comparison.png)

![Final Results](https://github.com/Shubhkirti24/SpicyCloud/blob/main/Results_spicy_cloud.png)

---




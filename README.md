Certainly! Here is an updated README file with more detailed information about model selection:

---

# Mushroom Edibility Prediction

This project investigates and compares the performance of three popular machine learning algorithms—logistic regression, decision trees, and random forests—in predicting the edibility of mushrooms based on their visual and olfactory characteristics.

## Table of Contents

- [Introduction](#introduction)
- [Data Description](#data-description)
- [Algorithms](#algorithms)
- [Model Statistics](#model-statistics)
- [Model Selection](#model-selection)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This report aims to determine whether a mushroom is edible or poisonous based on various features. The algorithms tested include logistic regression, decision trees, and random forests. The dataset includes several attributes describing the characteristics of mushrooms, which are used to predict their edibility.

## Data Description

The dataset contains six attributes that describe the characteristics of mushrooms. These attributes include:

1. **Edible**: Target variable indicating whether a mushroom is edible or poisonous.
2. **Cap Shape**: The shape of the mushroom cap (e.g., bell, conical, convex, flat, knobbed, sunken).
3. **Cap Surface**: The surface texture of the cap (e.g., fibrous, grooves, scaly, smooth).
4. **Cap Color**: The color of the cap (e.g., brown, buff, cinnamon, gray, green, pink, purple, red, white, yellow).

## Algorithms

The following machine learning algorithms were evaluated in this project:

1. **Logistic Regression**: A linear model for binary classification.
2. **Decision Trees**: A non-linear model that splits data based on feature values.
3. **Random Forests**: An ensemble method that combines multiple decision trees to improve performance.

## Model Statistics

### Logistic Regression Model
- **Accuracy**: 0.9957
- **Sensitivity (Recall)**: 0.9988
- **Specificity**: 0.9923
- **Positive Predictive Value (Precision)**: 0.9929
- **Negative Predictive Value**: 0.9987

### Decision Tree Model
- **Accuracy**: 0.9932
- **Sensitivity (Recall)**: 0.9964
- **Specificity**: 0.9898
- **Positive Predictive Value (Precision)**: 0.9905
- **Negative Predictive Value**: 0.9961

### Random Forest Model
- **Accuracy**: 0.9938
- **Sensitivity (Recall)**: 0.9952
- **Specificity**: 0.9923
- **Positive Predictive Value (Precision)**: 0.9929
- **Negative Predictive Value**: 0.9949

## Model Selection

In model selection, we assess different models to determine which one is most suitable for our task. There are several metrics that can help us make this decision:

1. **Accuracy**: Measures how often the model's predictions are correct overall. It is the ratio of correctly predicted instances to the total number of instances in the dataset. A higher accuracy means that the model is making more correct predictions.

2. **Sensitivity (Recall)**: Measures the model's ability to correctly identify positive instances. It focuses on how well the model detects the positive class (edible mushrooms). Higher sensitivity indicates that the model is better at identifying positive instances.

3. **Specificity**: Measures the model's ability to correctly identify negative instances. It focuses on how well the model distinguishes the negative class (poisonous mushrooms). Higher specificity indicates that the model is better at identifying negative instances.

4. **Positive Predictive Value (Precision)**: The proportion of positive predictions that are correct. High precision means that the model rarely misclassifies a negative instance as positive.

5. **Negative Predictive Value**: The proportion of negative predictions that are correct. High negative predictive value means that the model rarely misclassifies a positive instance as negative.

### Model Comparison

- **Logistic Regression**: This model achieved the highest accuracy, sensitivity, and specificity, making it the preferred choice for predicting mushroom edibility. It has the best balance of correctly identifying both edible and poisonous mushrooms.

- **Random Forest**: This model also performed well, with high accuracy, sensitivity, and specificity. It is a robust model that combines multiple decision trees to improve prediction performance.

- **Decision Tree**: While this model also achieved high accuracy, its sensitivity and specificity were slightly lower compared to logistic regression and random forest. It is still a good model but may not be as reliable as the other two.

### Conclusion

Based on these metrics, the Logistic Regression model performs better than the other models in terms of sensitivity, specificity, and accuracy. Therefore, the Logistic Regression model is the preferred choice for predicting the edibility of mushrooms.

## Results

### Model Accuracy Comparison
![Model Accuracy Comparison](accuracy_graph.png)

### Model Specificity Comparison
![Model Specificity Comparison](specificity_graph.png)

### Model Sensitivity Comparison
![Model Sensitivity Comparison](sensitivity_graph.png)

All three models have high accuracy, with the Logistic Regression model achieving the highest accuracy of 0.9957. However, the differences in accuracy between the models are relatively small.




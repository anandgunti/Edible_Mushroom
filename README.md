

# Mushroom Edibility Prediction

This project investigates and compares the performance of three machine learning algorithms—logistic regression, decision trees, and random forests—in predicting the edibility of mushrooms based on visual and olfactory characteristics.

## Table of Contents

- [Introduction](#introduction)
- [Data Description](#data-description)
- [Algorithms](#algorithms)
- [Model Statistics](#model-statistics)
- [Model Selection](#model-selection)
- [Results](#results)


## Introduction

The report investigates and compares the performance of three machine learning algorithms: logistic regression, decision trees, and random forests, in predicting the edibility of mushrooms based on visual and olfactory characteristics. The dataset includes several attributes describing the characteristics of mushrooms, which are used to predict their edibility.

## Data Description

The dataset contains six attributes that describe the characteristics of mushrooms:
1. **Edible**: Target variable indicating whether a mushroom is edible or poisonous.
2. **Cap Shape**: The shape of the mushroom cap (e.g., bell, conical, convex, flat, knobbed, sunken).
3. **Cap Surface**: The surface texture of the cap (e.g., fibrous, grooves, scaly, smooth).
4. **Cap Color**: The color of the cap (e.g., brown, buff, cinnamon, gray, green, pink, purple, red, white, yellow).
5. **Odor**: The odor of the mushroom (e.g., almond, anise, creosote, fishy, foul, musty, none, pungent, spicy).
6. **Height**: The height of the mushroom.
   
<img width="244" alt="d" src="https://github.com/anandgunti/Edible_Mushroom/assets/25959661/cc583a0b-7dac-44cd-bd01-18c457a4501e">

Converting variables to factors in R facilitates efficient handling of categorical data for machine learning algorithms designed for such data. Visualizing data distributions helps identify patterns, such as:
- Conical cap shapes are often poisonous, while sunken shapes are usually edible.
- Green or purple cap colors are typically edible.
- Odors like almond or anise are linked to edible mushrooms.

## Algorithms

The following machine learning algorithms were evaluated in this project:

1. **Logistic Regression**: A linear model for binary classification. Further tuning with methods like GLMNET enhanced its accuracy to 99.57% by selecting specific features.

  <img width="419" alt="1111" src="https://github.com/anandgunti/Edible_Mushroom/assets/25959661/b4a1b605-382c-48dd-a7dc-e2b7609b96c5">
Fine Tuning using cross-validation method 

2. **Decision Trees**: Non-linear models that split data based on feature values. Various models like rpart, C5.0, and ctree were explored, with C5.0 achieving the highest accuracy of 99.26% post-tuning.
3. **Random Forests**: Ensemble methods that combine multiple decision trees to improve performance. Models like wsrf and rf were used, with the rf model showing better accuracy at 99.08%.

## Model Statistics

### Logistic Regression Model
- **Accuracy**: 0.9957
- **Sensitivity (Recall)**: 0.9988
- **Specificity**: 0.9923
- **Positive Predictive Value (Precision)**: 0.9929
- **Negative Predictive Value**: 0.9987

### Decision Tree Model (C5.0)
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

In model selection, we assess different models to determine which one is most suitable for our task. The evaluation metrics include:

1. **Accuracy**: Measures how often the model's predictions are correct overall. It is the ratio of correctly predicted instances to the total number of instances in the dataset. A higher accuracy means that the model is making more correct predictions.

2. **Sensitivity (Recall)**: Measures the model's ability to correctly identify positive instances (edible mushrooms). Higher sensitivity indicates that the model is better at identifying positive instances.

3. **Specificity**: Measures the model's ability to correctly identify negative instances (poisonous mushrooms). Higher specificity indicates that the model is better at identifying negative instances.

4. **Positive Predictive Value (Precision)**: The proportion of positive predictions that are correct. High precision means that the model rarely misclassifies a negative instance as positive.

5. **Negative Predictive Value**: The proportion of negative predictions that are correct. High negative predictive value means that the model rarely misclassifies a positive instance as negative.

### Model Comparison

- **Logistic Regression**: Achieved the highest accuracy, sensitivity, and specificity, making it the preferred choice for predicting mushroom edibility. It has the best balance of correctly identifying both edible and poisonous mushrooms.
- **Random Forest**: Performed well, with high accuracy, sensitivity, and specificity. It is a robust model that combines multiple decision trees to improve prediction performance.
- **Decision Tree (C5.0)**: Achieved high accuracy but its sensitivity and specificity were slightly lower compared to logistic regression and random forest. It is still a good model but may not be as reliable as the other two.

### Conclusion

Based on these metrics, the Logistic Regression model performs better than the other models in terms of sensitivity, specificity, and accuracy. Therefore, the Logistic Regression model is the preferred choice for predicting the edibility of mushrooms.

## Results

### Model Accuracy Comparison
<img width="344" alt="222" src="https://github.com/anandgunti/Edible_Mushroom/assets/25959661/37bc370e-ff5f-474a-aaff-f9715eb2e45a">

### Model Specificity Comparison
<img width="357" alt="3333" src="https://github.com/anandgunti/Edible_Mushroom/assets/25959661/1764e5e2-d60d-4aa0-a768-aab1f71697d2">


### Model Sensitivity Comparison
<img width="329" alt="3" src="https://github.com/anandgunti/Edible_Mushroom/assets/25959661/79931574-8a55-4c24-9249-993da34f37ed">

All three models have high accuracy, with the Logistic Regression model achieving the highest accuracy of 0.9957. However, the differences in accuracy between the models are relatively small.



---

# Mushroom Edibility Prediction

This project investigates and compares the performance of three popular machine learning algorithms—logistic regression, decision trees, and random forests—in predicting the edibility of mushrooms based on their visual and olfactory characteristics.

## Table of Contents

- [Introduction](#introduction)
- [Data Description](#data-description)
- [Algorithms](#algorithms)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)


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

## Results

The performance of the algorithms is compared based on accuracy, precision, recall, and F1-score. Detailed results and visualizations can be found in the report.

## Usage

To run the code and reproduce the results, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/mushroom-edibility-prediction.git
    cd mushroom-edibility-prediction
    ```

2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the analysis script:
    ```bash
    python analysis.py
    ```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.


---

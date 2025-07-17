# Milk Quality Classification using CNN

## Problem Statement

Ensuring the quality of milk is a critical task in the food and dairy industry. Traditional methods rely on manual inspection and lab testing, which are time-consuming and may introduce human bias. To address this, we aim to build a **Convolutional Neural Network (CNN)** based classification model that can predict the **Grade** of milk (Low, Medium, or High) based on its physicochemical and sensory attributes.

## Objective

Develop a deep learning model using **Convolutional Neural Networks (CNN)** to classify milk into one of three quality grades: **Low (Bad), Medium (Moderate), or High (Good)** using a structured dataset of milk attributes.

## Dataset Description

The dataset contains various features representing the milk's quality parameters:

| Column Name  | Description                                        | Type        | Range/Values      |
| ------------ | -------------------------------------------------- | ----------- | ----------------- |
| `pH`         | pH value of the milk                               | Numerical   | 3.0 – 9.5         |
| `Temprature` | Temperature of the milk (in °C)                    | Numerical   | 34.0 – 90.0       |
| `Taste`      | Taste of the milk                                  | Categorical | 0 = Bad, 1 = Good |
| `Odor`       | Odor of the milk                                   | Categorical | 0 = Bad, 1 = Good |
| `Fat`        | Fat content                                        | Categorical | 0 = Low, 1 = High |
| `Turbidity`  | Turbidity level                                    | Categorical | 0 = Low, 1 = High |
| `Colour`     | Colour intensity of the milk (measured on a scale) | Numerical   | 240 – 255         |
| `Grade`      | **Target variable**: Quality grade of the milk     | Categorical | Low, Medium, High |

## Why CNN?

While CNNs are primarily used for image data, this project aims to explore the potential of using **1D CNNs** for structured/tabular data. CNNs can learn local patterns across features, potentially capturing subtle interactions better than traditional models.

## Tasks

1. **Data Preprocessing**

   - Encode categorical features if necessary.
   - Normalize numerical columns.
   - Convert the tabular data into a format compatible with 1D CNN input.

2. **Model Building**

   - Design and train a 1D CNN architecture.
   - Experiment with hyperparameters and layers (Conv1D, MaxPooling1D, Flatten, Dense).

3. **Evaluation**

   - Evaluate the model using accuracy, precision, recall, and F1-score.
   - Use confusion matrix to understand class-wise performance.

4. **Deployment (Optional)**

   - Build a simple UI to input new milk sample data and predict its grade.

## Expected Outcome

A working deep learning model that can classify milk samples into Low, Medium, or High quality with high accuracy using CNN-based architecture.

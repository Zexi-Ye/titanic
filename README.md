# Titanic Survivor Prediction Project

**Author:** Zexi Ye

**Date:** April 2020

## Introduction

<img src='img/titanic.jpg'>

Here is a brief overview of the background.
<blockquote>
The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.
</blockquote>

The goal of the project is, therefore, to develop a wide array of machine learning models that make prediction regarding whether a passenger would survive or not based upon engineered features.

## Repo Structure

- **data**: Contains the raw data (train and test) as well as the randomly split training set and validation set used in the course of training. <font color='blue'>train.csv</font> consists of both features and target (Survived), while <font color='blue'>test.csv</font> consists of features only.

- **models**: Contains the trained models as pickle files. You may find 6 smodels stored under this directory.

- **output**: Contains the predictions on the test data given by various trained models.

- **img**: Contains source images to be displayed in the notebook.

## Core Content

The notebook **Titanic Project.ipynb** provides a fairly detailed documentation of every step in this project, so please view the notebook if you are interested.

## Results

Our models will be evaluated on the test set using accuracy as the metric. Results will be compared to the baseline, which already achieves a decent accuracy.

**Baseline**: Classify all males as not survived and all females as survived.

Below is a table of test accuracies associated with the models.

|Model|Accuracy|
|---|---|
|Gradient Boosting|79.904%|
|Logistic Regression|79.425%|
|SVM|78.947%|
|KNN|76.555%|
|*Baseline|76.555%|
|Random Forest|76.076%|
|Blending|75.119%|
|Naive Bayes|75.119%|

Note that the best score is **79.904%**, given by the gradient boosting trees classifier, which is an improvement of **3.349%** with respect to the baseline model. Arguably, the test score could potentially be enhanced through finer feature engineering (e.g. additional features) as well as more sophisticated machine learning algorithms.
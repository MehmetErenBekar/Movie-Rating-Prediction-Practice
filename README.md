# Movie Rating Prediction

A machine learning practice project analyzing movie data to predict ratings 
using both regression and classification approaches, with model comparison 
via cross-validation.

## Overview

This project explores a movie dataset to:
1. Predict exact IMDB ratings using regression (Phase 1)
2. Classify movies as "good" or "bad" using classification (Phase 2)
3. Compare multiple models using cross-validation for reliable evaluation (Phase 3)

## Dataset

The dataset includes movie attributes such as runtime, vote count, gross earnings, 
and genre, used to predict movie ratings.

## Phase 1 — Regression

**Model:** Linear Regression  
**Features:** runtime, votes, gross earnings  
**Results:**
- MAE: [senin sayın]
- RMSE: [senin sayın]

A scatter plot of actual vs. predicted ratings shows [kısa yorum].

## Phase 2 — Classification

Ratings were converted into a binary label (good movie ≥ 7.0, bad movie < 7.0). 
Genre was one-hot encoded as an additional feature set.

**Model:** Logistic Regression  
**Results:**
- Accuracy: [senin sayın]
- Precision: [senin sayın]
- Recall: [senin sayın]
- F1 Score: [senin sayın]

Confusion matrix visualization included in the notebook.

## Phase 3 — Model Comparison with Cross-Validation

Three models were compared using 5-fold stratified cross-validation with F1 scoring:

| Model                | F1 Score |
|----------------------|----------|
| Logistic Regression   | 0.7196  |
| KNN                    | 0.6430  |
| Decision Tree          | 0.6400  |

Cross-validation was used instead of a single train/test split to get a more 
reliable estimate of model performance, since a single split can be affected 
by how the data happens to be divided.

## Tech Stack

- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

## Key Learnings

- Feature scaling matters for distance-based models (KNN) but not for tree-based models
- A single train/test split can give misleadingly optimistic (or pessimistic) results — 
  cross-validation gives a more trustworthy picture
- Encoding categorical variables (genre) via one-hot encoding for multi-label features


Mehmet Eren Bekar

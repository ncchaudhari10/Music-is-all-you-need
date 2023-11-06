# Music Genre Classification Kaggle Competition - Music is all you need!

## Overview

This repository contains the code and resources for my participation in the [Music Genre Classification Kaggle competition](https://www.kaggle.com/competitions/music-vibes-datathon-fall23/overview). The competition's goal was to improve the music discovery experience by accurately classifying the genre of songs based on their attributes. I used a CatBoostClassifier and data preprocessing techniques to achieve competitive results.

## Dataset

The dataset for this competition included rich information about songs, such as track names, album names, artist names, release dates, and various audio features. The 'target' variable represented the genre of each song.

## Solution Scores

- Private Score: 0.73788
- Public Score: 0.72223


## Code Structure

- `data/`: Contains the dataset files.
- `notebooks/`: Jupyter notebooks for data exploration, preprocessing, model development, and evaluation.

## Workflow

1. **Data Preprocessing**: I loaded and preprocessed the data, including handling missing values, converting date formats, and feature selection. I also performed over-sampling using SMOTENC to address class imbalance.

2. **Hyperparameter Optimization**: I used Optuna to optimize the hyperparameters for the CatBoostClassifier, aiming to maximize accuracy. The best hyperparameters were used for training.

3. **Model Training**: The CatBoostClassifier was trained on the resampled data using the optimized hyperparameters.

4. **Feature Importance**: I analyzed feature importance and identified the top features that contributed to the model's predictions.

5. **Prediction**: I made predictions on the test data and saved the results in the `submission.csv` file.

## Results

- The competition's evaluation metric was the F1 score. The weighted F1 score for the submission is [insert score here].
- During the competition, I observed that the performance of the model improved significantly after handling missing values and over-sampling.
- Challenges faced included dealing with a small imbalanced dataset, tuning hyperparameters effectively, and selecting the most relevant features from a wide range of data.

## Areas for Improvement

- Experiment with other classification algorithms to potentially improve model performance.
- Fine-tune hyperparameters and optimize for specific metrics or objectives.
- Apply advanced techniques for dealing with imbalanced data to improve model robustness.


# Multi-Class-Prediction-of-Cirrhosis-Outcomes

## Overview

In this Playground Series - Season 3, Episode 26 on Kaggle, we seek to build a model that predict the probability of a patient's disease using many features.

## Table of Contents

- [Multi-Class Prediction of Cirrhosis Outcomes](#Multi-Class Prediction of Cirrhosis Outcomes)
  - [Overview](#overview)
  - [Table of Contents](#table-of-contents)
  - [Files and Directory Structure](#files-and-directory-structure)
  - [Dependencies](#dependencies)
  - [Model Architecture](#model-architecture)
  - [Results](#results)
  - [Issues and Future Improvements](#issues-and-future-improvements)

## Overview

As always, the goal is to goal is to craft a white/black bow that minimizes the loss on the test loss.
The first thing I sough to accomplish is to clean my data, that is, to fill missing numbers, and convert all to numerical data.

I finished by OneHot Encoding all the features, cause it's always better.

In th

## Files and Directory Structure

Explain the organization of your project files and directories.

```plaintext
|-- /data
|   |-- [Your dataset files]
|-- /notebooks
|   |-- your_model_creation_notebook.ipynb
|-- /src
|   |-- [Your source code files]
|-- README.md
|-- requirements.txt
|-- [Other project files]
```

## Dependencies
I opted to use pycaret, a library that compares and ranks many state-of-the-art models on your data, and optuna, a newly-discovered library used to optimize my model.
There's no need to talk about other libraries such as sklearn, scipy, matplotlib, seaborn, etc.

## Model Architecture
I opted for stacking, a highly used ml model architecture that combines heterogenous models, and aggregated by training a meta-learner: Another model that learns the best aggregating weights that minimize the stacking model on train model.

## Result
![Multi-Class-Prediction-of-Cirrhosis-Outcomes](/workspaces/Multi-Class-Prediction-of-Cirrhosis-Outcomes/images/ranking.png)
As you can see, I ranked top 38% up-to-day

## Issues and Future Improvements

Numerous approaches could be adopted to improve the accuracy of this model:
    - Feature engineering
    - hyperparameter optimization using optuna
    - eventually using a NN
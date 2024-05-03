# Machine Learning Model for Performance Prediction

## Introduction
This project focuses on developing a machine learning model to predict the performance of configurations based on various features extracted from data files. We use LightGBM's ranking model to assess the impact of configurations on performance.

## Data Preparation
The data used in this project resides in the `./data/tpugraphs/npz/tile/xla` directory. Each data file contains multiple features which are pre-processed and sampled for training the model.

## Model Training
* We employ a `LightGBM Ranker` to train our model. The ranker uses features such as node characteristics and configuration parameters to predict the performance ranks within different groups.
* The model's predictions are evaluated against a baseline to check the effectiveness of different configurations. The performance is measured by how well the model can predict the best configurations.

## Directory Structure
- `data/`: Contains the datasets in `.npz` format.
- `scripts/`: Contains the source code.

## Output
The predictions are saved in `result_xla.csv`, which contains the configurations predicted to perform best.

# Sepsis-Prediction
Sepsis Prediction using Clinical Data (PhysioNet Computing in Cardiology Challenge 2019)

This project implements an LSTM-based sepsis prediction model using various clinical data sources. Specifically, the model takes 10 hours of input data and predicts the probability of sepsis within the next hour.

The data used for this project is from the 2019 PhysioNet Computing in Cardiology Challenge. The following link provides more information about the data and a link to download: https://physionet.org/content/challenge-2019/1.0.0/

The dataset is a series of PSV files, where each row represents a single hour of data. 

To run the code in this project, run the following notebooks:
1. `psv_to_df.ipynb`: This notebook loads the PhysioNet data PSV files and saves them into a Pandas DataFrame for ease of downstream analysis
2. `feature_engineering.ipynb`: This notebook generates 10 hour-windowed features and corresponding labels
3. `feature_selection.ipynb`: This notebook inspects feature correlations and removes any features that are highly correlated
4. `train_model.ipynb`: This notebook defines the model, trains it, and evaluates its performance on validation and test sets

# Impulse_hackathon-
'''
Project Documentation: EEG Classification Using Machine Learning
Objective:
To develop a machine learning solution for classifying EEG data based on extracted features and achieving high classification accuracy.

Steps Followed:
1. Understanding the Problem Statement
Analyzed the provided EEG Dataset and problem requirements.
Noted that the dataset includes .npy files with EEG signals and a sample output file (sample_test_output.csv).
2. Dataset Preparation
Located and loaded the dataset folders: train_data, validation_data, and test_data.
Inspected the data for shape, structure, and label distribution.
Addressed Missing Labels by linking sample_test_output.csv for test labels.
3. Preprocessing the Data
Applied Bandpass Filtering to isolate relevant EEG frequencies.
Experimented with Wavelet Denoising but decided to proceed with filtering for simplicity.
Normalized the EEG data to prepare it for feature extraction.
4. Feature Extraction
Extracted frequency-domain features (e.g., power in alpha and beta bands).
Performed wavelet decomposition to capture time-frequency characteristics.
Computed statistical features like mean, variance, and standard deviation for each EEG channel.
5. Baseline Model Development
Built a simple Random Forest Classifier as the baseline model.
Trained the model using extracted features and evaluated its performance.
Achieved a baseline accuracy of ~56% with the initial feature set.
6. Advanced Model Building
Designed a hybrid CNN-LSTM model to capture both spatial and temporal dependencies in EEG signals.
Tuned hyperparameters, including learning rate, batch size, and number of epochs, for optimal results.
Incorporated class weighting to handle label imbalances in the dataset.
7. Evaluation and Improvements
Evaluated models using accuracy, classification reports, and confusion matrices.
Experimented with advanced techniques:
SHAP analysis to identify important features.
Feature selection to focus on significant predictors.
Applied oversampling and class balancing for improved generalization.
8. Test Data Predictions
Processed the test dataset and generated predictions.
Saved the output in the required CSV format (final_test_output.csv).
'''

'''
I developed two models for task 7 
the first model use hybrid CNN-LSTM model, designed to capture both spatial and temporal patterns in the EEG data.
With a highest accuracy Approximately of 94.81% and Test Accuracy Around 35.94%.
The second model uses Random Forest Classifier with highest accuracy of 100.0%
'''

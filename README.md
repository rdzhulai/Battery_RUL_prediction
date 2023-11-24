# Model Documentation

## 1. Overview

This documentation outlines the details of a linear regression model developed to predict the remaining useful life (RUL) of NMC-LCO 18650 batteries based on features derived from their voltage and current behavior over multiple cycles. The dataset used for training and evaluation was obtained from the Hawaii Natural Energy Institute, comprising 14 batteries cycled 1000 times at 25°C with a CC-CV charge rate of C/2 and discharge rate of 1.5C. The dataset can be found on [Kaggle](https://www.kaggle.com/datasets/ignaciovinuales/battery-remaining-useful-life-rul?select=Battery_RUL.csv).

## 2. Motivation

The aim is to create a predictive model that can estimate the remaining useful life of batteries, providing insights into their degradation over cycles. This information is valuable for proactive maintenance and optimal utilization of battery systems.

## 3. Success Metrics

The success of the model is primarily evaluated using the Root Mean Squared Error (RMSE) as a performance metric, measuring the accuracy of the predicted RUL compared to the actual values.

## 4. Requirements & Constraints

### 4.1 What's in-scope & out-of-scope?

In-scope:
- Training a linear regression model for RUL prediction.
- Evaluation of model performance using RMSE.

Out-of-scope:
- Implementation of complex machine learning techniques beyond linear regression.

## 5. Methodology

### 5.1. Problem Statement

The problem involves predicting the remaining useful life of batteries based on voltage and current behavior features extracted from cycling data.

### 5.2. Data

The dataset includes variables such as cycle index, discharge time, time at 4.15V, time constant current, and others.

### 5.3. Techniques

A linear regression model is employed, considering the simplicity and interpretability of the model for this problem.

### 5.4. Experimentation & Validation

The model is trained and validated using a train-test split, and performance is evaluated using RMSE.

## 6. Implementation

### 6.1. High-level Design

The implementation follows a standard machine learning workflow, involving data loading, exploration, model training, prediction, and evaluation.

### 6.2. Infra

No specific infrastructure requirements beyond a Python environment with necessary libraries.

### 6.3. Performance (Throughput, Latency)

Not applicable for this offline prediction task.

### 6.4. Security

No security considerations are relevant for this model.

### 6.5. Data Privacy

The dataset is assumed to be anonymized, and no specific privacy concerns are addressed.

### 6.6. Monitoring & Alarms

No real-time monitoring or alarms are implemented for this offline model.

### 6.7. Cost

The cost of model development and execution is minimal, considering it's a linear regression model with no elaborate infrastructure requirements.

### 6.8. Integration Points

The model integrates with the input data containing battery features for prediction.

### 6.9. Risks & Uncertainties

Risks include potential model overfitting and limitations of a linear regression approach. Uncertainties may arise from the variability in battery behavior.

## 7. Appendix

### 7.1. Alternatives

Consideration was given to more complex models, but the simplicity and interpretability of linear regression were deemed suitable.

### 7.2. Experiment Results

RMSE is used as the primary metric, and the current value is 7.024.

### 7.3. Performance Benchmarks

No specific performance benchmarks are established beyond RMSE.

### 7.4. Milestones & Timeline

The model development timeline involves data preparation, training, and evaluation.

### 7.5. Glossary

- RUL: Remaining Useful Life
- RMSE: Root Mean Squared Error

### 7.6. References

No external references were consulted for this specific model.
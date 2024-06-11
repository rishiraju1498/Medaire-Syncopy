# Medaire: Unexpected Fainting Events
## Project Overview

This project, conducted by the ASU Team, aims to understand the causes and patterns of fainting incidents during flights. The goal is to enhance MedAire's medical guidance for airlines, improve passenger experience, and avoid unnecessary flight diversions.

## Project Objective

Passengers frequently faint during flights, leading to unnecessary medical responses and flight diversions. Understanding these incidents is crucial for MedAire to provide better medical guidance to airlines.

### Emergency Landing Cost

- Estimated cost: $10k to $300k (Approx.)

## Risks & Issues

### Lack of Complete Data

- Incomplete analysis and potentially skewed findings.
- Missing data for TifMin and TeleMedicine kit availability.
- Complexity of fainting incidents due to environmental factors.
- Need for comprehensive medical data for thorough modeling.
- Insufficient and imbalanced sample size.
- Fainting incidents account for only 11% of all flight diversions.

## Exploratory Data Analysis

### Tableau Dashboard Insights

- **Acft Family**: Maximum diversions in B737 flights followed by A319.
- **Acft Type**: Maximum diversions in Narrow Body flights.
- **Div Initiated By**: 60% of cases initiated by MedLink.
- **Domlnt**: Maximum diversions in international flights.
- **Final Patient Disp**: Most patients taken to the hospital.
- **Haul IATA**: Most diversions in Long Haul flights, followed by Medium Haul flights.
- **Diagn Categ**: Most cases are Neurological, followed by Cardiovascular.
- **Diag Impression**: Most cases due to fainting, followed by chest pain.
- **Altitude**: Maximum diversions occur at altitudes ranging 30K-35K.

## Literature Review

- Common Causes: Drop in BP, Diabetes, Alcoholism, Medication, Low Oxygen
- Prevalence: 30% inflight medical events are fainting events but they contribute to 70% of flight diversions
- Management Strategy: Canadian Syncope Risk Score, Positioning the person in the aisle, Prevention strategies

## Data Cleaning and Adding Calculated Fields

- Calculated great circular distance field.
- Standardized patient age to years.
- Eliminated irrelevant columns and null values.
- Implemented imputation techniques (Mean for numerical data, Mode for categorical data).

### Data Pre-Processing

- **One-Hot Encoding**: Converted categorical columns into binary representations.
- **SMOTE (Synthetic Minority Over-sampling Technique)**: Addressed class imbalance by generating synthetic samples for underrepresented classes.

## Results

### Prediction of Diversion for Syncope Events

- **Decision Tree Model**: Accuracy - Class 0: 97.90%, Class 1: 57%
- **Random Forest Model**: Accuracy - Class 0: 97.90%, Class 1: 60%

## Future Work

- Implement wearable technology for real-time monitoring of passengers' vital signs.
- Investigate psychological aspects like anxiety and stress related to flying.

## Conclusion

- **Patient Age & Altitude**: Significant factors in fainting incidents and flight diversions.
- **Long Flights**: Indicated by total flight minutes and great circular distance.
- **Narrow Body**: Potential for claustrophobia leading to fainting.
- **Medical Volunteer**: Presence leads to more diversions.
- **Flight Halt Time**: Average diverted flight halt time is 2 hours.

## Thank You!

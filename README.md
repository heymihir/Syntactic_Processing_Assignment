# Custom Named Entity Recognition (NER) for Medical Data

## Overview

This project focuses on creating a custom Named Entity Recognition (NER) model to identify diseases and treatments within medical text data. The model is built using Conditional Random Fields (CRF) and leverages the spaCy library for natural language processing.

## Major Tasks

### 1. Data Preprocessing
- **Objective:** Convert word-level data into sentence-level data.
- **Steps:**
  - Construct sentences from individual words.
  - Ensure correct counts of sentences and labels.

### 2. Concept Identification
- **Objective:** Identify key concepts in the dataset.
- **Steps:**
  - Use Part-of-Speech (PoS) tagging to extract tokens tagged as NOUN or PROPN.
  - Print the top 25 most common NOUN/PROPN tokens.

### 3. Defining Features for CRF
- **Objective:** Define features for the CRF model.
- **Steps:**
  - Include PoS tags and preceding word information.
  - Mark the beginning and end of sentences.

### 4. Getting Features and Labels
- **Objective:** Extract features and labels for each sentence.
- **Steps:**
  - Write code to get feature values for each sentence.
  - Write code to get labels for each preprocessed label line.

### 5. Defining Input and Target Variables
- **Objective:** Prepare input and target variables for the CRF model.
- **Steps:**
  - Extract feature values for each sentence in train and test datasets.
  - Extract labels as target variables.

### 6. Building the Model
- **Objective:** Build the CRF model for NER.
- **Steps:**
  - Use the defined features and target variables to train the model.

### 7. Model Evaluation
- **Objective:** Evaluate the performance of the model.
- **Steps:**
  - Predict labels for the test dataset.
  - Calculate the F1 score using actual and predicted labels.

### 8. Identifying Diseases and Treatments
- **Objective:** Identify diseases and their corresponding treatments.
- **Steps:**
  - Create a dictionary mapping diseases to treatments from the test dataset.
  - Predict treatments for a specific disease (e.g., 'hereditary retinoblastoma').
## SKYHACK 2.0
# United Airlines Call Center Optimization

## Table of Contents
1. [Project Overview](#project-overview)
2. [Problem Statement](#problem-statement)
3. [Background](#background)
4. [Data Preprocessing](#data-preprocessing)
5. [Model Building & Tuning](#model-building--tuning)
6. [Predictions](#predictions)

7. [Results](#results)
8. [Conclusion](#conclusion)
9. [References](#references)

---

## Project Overview
This project focuses on analyzing United Airlines call center data to optimize key performance metrics like Average Handle Time (AHT) and Average Speed to Answer (AST). The findings will help streamline call center operations, enhancing customer service efficiency.

---

## Problem Statement
United Airlines aims to improve its call center operations by reducing AHT and AST while ensuring customer satisfaction. This project involves analyzing data to identify inefficiencies, determining causes of long AHT and AST, and recommending strategies for improving performance.

---

## Background
Call centers are crucial for addressing customer inquiries, complaints, and service requests. The primary challenge is optimizing the balance between human agents and IVR systems to minimize AHT and AST while meeting customer needs.

### Key Metrics:
- *Average Handle Time (AHT):* Total time spent on a call by an agent.
  - Formula: AHT = Total Handle Time / Total Number of Calls
- *Average Speed to Answer (AST):* Time spent by customers in the queue before an agent answers.
  - Formula: AST = Total Waiting Time / Total Number of Calls

---

## Data Preprocessing
The dataset provided includes various call center metrics, which required cleaning and preprocessing.

### Steps:
1. *Text Cleaning:*
   - Standardized and generalized the text data using regex.
   - Function text_cleaning() cleans the data by removing special characters and formatting text.

2. *Text Formatting:*
   - Capitalized the first letter of each word using capitalize_text() function.

3. *Feature Selection:*
   - Selected relevant features: call_id, average_sentiment, call_hour, AHT, AST, and primary_call_reason.

4. *Label Encoding:*
   - Encoded the target variable (primary_call_reason) using LabelEncoder.

### Model Building & Tuning
A Random Forest classifier was used to predict the primary call reason, and hyperparameter tuning was conducted using GridSearchCV.

Code & Instructions
Requirements:
Python 3.x
Required libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

The output file test_orfolks.csv will contain the predicted results.



## Conclusion
Our analysis identified key factors contributing to long AHT and AST. We recommend improving self-service IVR options to reduce agent involvement and optimizing call handling processes.

## References
Call center dataset provided by United Airlines.
Python libraries: pandas, scikit-learn, seaborn.

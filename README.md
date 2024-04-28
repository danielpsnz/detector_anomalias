#  Detection of Credit Card Fraud

## Overview:
This repository contains a data science project aimed at addressing issues related to credit card fraud within a consumer finance company belonging to one of Spain's top five banks. The operations department has reported numerous instances of credit card duplication and a surge in fraudulent transfers. To tackle this problem, they seek assistance in developing a statistical model.

Fraudulent activities in consumer finance, particularly in credit cards, pose a significant challenge to the financial sector, leading to both monetary losses and a decline in customer trust and loyalty. Detecting and preventing such fraudulent transactions is crucial for maintaining the integrity of the financial system.

## Context:
In real-world scenarios, unsupervised algorithms are often employed to identify anomalous transactions from the entire dataset. While some businesses use predefined rules to filter out anomalies, these rules can be complex to formulate. Hence, unsupervised models that can flag suspicious behaviors provide a valuable initial screening mechanism. By extracting features from each transaction (X) and utilizing anomaly detection algorithms, anomalous transactions can be identified and distinguished from normal ones.

Subsequently, all flagged anomalous transactions undergo auditing to obtain the actual labels (Y), distinguishing between fraudulent (Y=1) and non-fraudulent (Y=0) transactions. With labeled data (X,Y) available, a supervised learning classifier can be constructed by the financial institution.

## Problem Statement:
In this project, we have access to the features of each transaction (X) along with labels indicating fraud or non-fraud (Y). While a supervised learning classifier could be directly constructed, the objective is to explore the utility of an anomaly detection model in preliminary stages.

We will assume the absence of labels (Y) and develop an anomaly detection model solely based on features (X). By identifying anomalous transactions and comparing them with actual labels (Y), we aim to assess how an anomaly detector could aid in the initial screening process.

## Objectives:
* Data reading and initial analysis, including the number of rows, columns, and variable names.
* Dataset division into training and testing sets.
* Visualization of data using PCA models with two and three components, distinguishing between fraudulent and non-fraudulent transactions.
* Fitting a local outlier factor (LOF) anomaly detection model.
* Assigning the top 2% most anomalous data points to class 0 and the bottom 98% to class 1.
* Comparative analysis of the performance gain achieved using the anomaly detection model versus not using it, potentially utilizing cumulative gain representation for evaluation.

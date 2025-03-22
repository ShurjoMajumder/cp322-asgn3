---
title: "Assignment 3 Master Report"
date: "21 Mar 2025"
author: 
  - "Shurjo Majumder (ID: 169035249)"
  - "Robin Chen (ID: 210178740)"
geometry: margin=2cm
classoption:
- twocolumn
---

## Part 1: 

> Completed By: Shurjo Majumder

### Introduction

In this part, an ANN was trained to classify hand written digits using the MNIST dataset.

### Performance Summary

Validation scores:

Confusion matrix of best model:

### Adjusting Hyperparameters

Increasing batch size decreased time to converge. Increasing learning rate lowered accuracy. The best hidden layer count was (64, 64), as more led to overfit, while fewer led to underfit.

### Conclusion

## Part 2: Naïve Bayes Classifier

> Completed By: Robin Chen

### Introduction

In this part of the assignment, a Naïve Bayes classifier was implemented to classify real vs. fake news headlines. The dataset consisted of 1298 fake news headlines and 1968 real news headlines. The text data was preprocessed and converted into numerical features using CountVectorizer. The dataset was split into 70% training and 30% testing sets.

### Performance Summary

The following results were recorded during testing, showing the accuracy and confusion matrix of the Naïve Bayes classifier:

Test Accuracy: 0.7898

Confusion Matrix:

```
[[287  95]
 [111 487]]
```

### Final Accuracy & Model Performance
The final accuracy achieved was 78.98%, indicating that the Naïve Bayes classifier performed reasonably well in distinguishing between real and fake news headlines. The confusion matrix provides further insights into the model's performance:

True Negatives (TN): 287 (fake news correctly classified as fake)

False Positives (FP): 95 (fake news incorrectly classified as real)

False Negatives (FN): 111 (real news incorrectly classified as fake)

True Positives (TP): 487 (real news correctly classified as real)

The model demonstrated a higher accuracy in classifying real news (81.4%) compared to fake news (75.1%). This suggests that the classifier is more effective at identifying real news headlines, while it struggles slightly more with fake news headlines.

### Conclusion
The Naïve Bayes classifier achieved a final accuracy of 78.98%, indicating a decent performance in classifying real and fake news headlines. The confusion matrix highlights the model's strengths in identifying real news and its challenges in accurately classifying fake news. Overall, the model provides a solid baseline for text classification tasks.

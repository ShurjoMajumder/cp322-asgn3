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

Lower learning rates during training tended to perform better, declining rapidly after $\lambda = 10^{-2}$.


This was a model with hidden units (64, 64), and batches set to be automatically sized, $\lambda = 10^{-3}$. 

![Validation Accuracy to Learning Rate](../assets/validation.png)

![Confusion Matrix](../assets/confusion_matrix.png)

### Adjusting Hyperparameters

Increasing batch size decreased time to converge. The best batch size was determined by simply setting the batch size in the model to "auto". Increasing learning rate lowered accuracy. The best hidden layer count was (64, 64), as more led to overfit, while fewer led to underfit.

In this case chose the best batch size and hidden layer hyperparameters by praying to Saraswati that the values I choose are the best ones, then pick arbitrary values after multiple training cycles. If I had unlimited computational resources, I'd run a more exhaustive grid search across many different batch sizes/learning rates/hidden unit counts and find which is truly optimal.

### Conclusion

In conclusion, the model displayed an overall accuracy of 96% over the test set. The confusion matrix shows that the likelihood of mis-classification is fairly low, and the model is remarkably accurate in identifying the "1" glyph.

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

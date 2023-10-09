# Chapter-7-exercises
This repository contains my solutions to the exercises in Chapter 7 'Ensemble Learning and Random Forests' of the book "Hands-On Machine Learning" by Aurélien Géron. The solutions are written in Python using the scikit-learn library. 
# MNIST Ensemble Learning and Stacking

In this repository, I have solved two exercises from Chapter 7 and Chapter 8 of the book "Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow" by Aurélien Géron. These exercises involve exploring ensemble learning techniques, including a voting classifier and stacking, to improve the performance of classifiers on the MNIST dataset.

## Exercise 8 - Ensemble Learning

### Objective
In Exercise 8, we load the MNIST dataset and split it into training, validation, and test sets. We then train various classifiers, such as a Random Forest classifier, an Extra-Trees classifier, and an SVM classifier. The goal is to combine them into an ensemble that outperforms each individual classifier on the validation set using soft or hard voting. Finally, we evaluate the ensemble on the test set and compare its performance to individual classifiers.

### Steps

1. Load the MNIST dataset and split it into training, validation, and test sets.
2. Train multiple classifiers, including a Random Forest classifier, an Extra-Trees classifier, and an SVM classifier.
3. Create an ensemble using soft or hard voting to combine the individual classifier predictions.
4. Evaluate the ensemble's performance on the validation set.
5. Test the ensemble on the test set and compare its performance to individual classifiers.

## Exercise 9 - Stacking Ensemble

### Objective
Exercise 9 focuses on building a stacking ensemble. We first run the individual classifiers from Exercise 8 to make predictions on the validation set. Then, we create a new training set with the resulting predictions, where each training instance is a vector containing the predictions from all classifiers for an image, and the target is the image's class. We train a classifier on this new training set, which acts as a blender. Finally, we evaluate the stacking ensemble on the test set and compare it to the voting classifier from Exercise 8.

### Steps

1. Use the individual classifiers trained in Exercise 8 to make predictions on the validation set.
2. Create a new training set with predictions from all classifiers as features and the image's class as the target.
3. Train a classifier (the blender) on this new training set.
4. For each image in the test set, make predictions with all individual classifiers.
5. Feed the predictions to the blender to obtain the ensemble's predictions.
6. Evaluate the stacking ensemble's performance on the test set and compare it to the voting classifier from Exercise 8.

## Conclusion

This repository contains the code and results for these two exercises. It demonstrates the power of ensemble learning techniques, including voting classifiers and stacking, in improving classification performance on the MNIST dataset. You can explore the code and experiment with different classifier combinations to gain a better understanding of ensemble learning in practice.

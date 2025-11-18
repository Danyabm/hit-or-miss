# Hit or Miss? Leveraging CPS for Sports Performance
Final Project for CS 6762: Signal Processing, Machine Learning, and Feedback Control

[Link to Slides](https://docs.google.com/presentation/d/1-CO4tv4fQTNYF__Va-ylBJvRSAP-KOniyRmFo4ujkXU/edit?usp=sharing) 

This project uses accelerometer and gyroscope data from a smartwatch to classify tennis strokes as either hits (racket–ball contact) or misses (swings without contact). The goal is to demonstrate how lightweight ML models can support sports performance analysis and real-time feedback.

**Methodology**

**Data Source**: ASUS ZenWatch 2 (Accel + Gyro)

**Activities**: Hit vs Miss swings, collected from two players

**Windowing**: 1s, 2s, 3s, 4s sliding windows

**Features**: Mean, median, standard deviation, RMS

**Models**: Random Forest, Logistic Regression, SVM

**Feature Selection**: Recursive Feature Elimination (RFE)


**Results**
_Model	Best Accuracy_
Random Forest	96.66%
Logistic Regression	96.52%
SVM	98.26%

SVM with a 4-second window achieved the highest accuracy, showing strong separation between hit and miss classes with minimal false predictions.


**Highlights**

High-accuracy classification using simple wearable sensors

Consistent performance across multiple time windows

Clear decision boundaries and strong generalization

Lightweight enough for real-time sports training applications


# Exploring Automatic Diagnosis of COVID-19 from Crowdsourced Respiratory Sound Data


## Paper link

https://dl.acm.org/doi/pdf/10.1145/3394486.3412865

## 	Date

August 23–27, 2020

## 	Feature extraction

1.	MFCC
2.	Δ-MFCC
3.	Δ2-MFCC
4.	Spectral Centroid
5.	Roll-off Frequency
6.	Zero-crossing
7.	RMS Energy
8.	VGGish

## 	Classifications

1.	Logistic Regression (LR)
2.	Gradient Boosting Trees
3.	Support Vector Machines (SVMs)
	We evaluated an SVM classifier with a Radial Basis Function (RBF) kernel

## 	Dataset

The dataset was collected through an app (Android and Web) that asked volunteers for samples of their voice, coughs and breathing as well as their medical history and symptoms. The app also asks if the user has tested positive for COVID-19. To date, we have collected on the order of 10,000 samples from about 7000 unique users

## 	Hyper parameters

1.	regularization parameter C
2.	kernel coefficient 𝛾

## 	Performance

models achieve an AUC of above 80% across all tasks

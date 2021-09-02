
# Robust Detection of COVID 19 in Cough Sounds

##	Paper link
https://link.springer.com/content/pdf/10.1007/s42979-020-00422-6.pdf

## 	Date
3 July 2020 / Accepted: 8 December 2020 / Published online: 12 January 2021.

## 	Features

1.	MFCC and 13 MFFC.
2.	Variable Markov Oracle (VMO).
3.	recurrence Quantification analysis (RQA).
4.	recurrence plot (RP).
5.	information rate (IR).

![covide1-1](https://user-images.githubusercontent.com/47793179/131899882-aaf75bce-c2a0-4b05-8755-9d391a4d85de.PNG)

## 	Classifications

1.	decision trees.
2.	 support vector machines.
3.	 K-nearest-neighbor.
4.	 random forest (RF).
5.	 XGBoost.

## 	Dataset

collected by the Corona Voice Detect project in partnership with Voca.ai and Carnegie Mellon University, samples include self-submitted audio recordings, age, gender, country of residence (optional), smoking habits (optional).

The dataset of cough samples consists of 1895 healthy and 32 sick samples, and the dataset of ’ah’ vowels consists of 1468 healthy and 20 sick samples.

## 	Algorithm

1.	SMOTE:

	SMOTE with data cleaning using the Wilson’s Edited Nearest Neighbor rule (SMOTE + ENN).
  
	SMOTE with data cleaning using Tomek Links (SMOTE + TL).

2.	ADASYN.
3.	Majority Weighted Minority Oversampling Technique (MWMOTE).
4.	NEATER.

## 	Performance

The proposed model achieves a mean classification performance of 97% and 99%, and a mean F1-score of 91% and 89% after optimization, for coughs and sustained vowels, respectively

![covide 1-2](https://user-images.githubusercontent.com/47793179/131900833-3be8c4b9-b9ca-451e-94e0-c34064724ea3.PNG)

![covide1-3](https://user-images.githubusercontent.com/47793179/131900871-99661ef4-5561-4cf7-b7b0-fa0411e9ea69.PNG)

![covide 1-4](https://user-images.githubusercontent.com/47793179/131900912-037d9e9a-b22a-4daf-8810-3c2b8f512567.PNG)

## 	Future Work

expand our analysis to other speech signals 
such as sustained vowels ’oh’ and ’eh’, as well as spontaneous speech signals


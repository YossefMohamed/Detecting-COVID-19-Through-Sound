Paper Link:

IEEE Articale

Date of publish 
12 July 2021

Classifications:

Recall COVID-19 positive (ACC+), also known as sensitivity, which is the true positive rate. 
Recall COVID-19 negative (ACC−), also known as specificity, which is the true negative rate.
Unweighted Average Recall (UAR): Also known as Unweighted Average Accuracy, is the average of sensitivity and specificity – the standard competition measure in the Interspeech ComParE challenge series. Chance level for two classes resembles 50.0 % UAR. 
Area Under ROC Curve (AUC): The ROC curve plots the true-positive rates against the false-positive rates with varying classification thresholds, and measures the area under the drawn curve. This measures how well a model can distinguish between the positive and negative classes, where a random baseline classifier will get a value of 50.0 %.
Accuracy (ACC): The ratio of examples that are answered correctly in the evaluation set.

Features:
ImageNet Large Scale Visual Recognition Challenge (ILSVRC)
SVM models to classify if a person have COVID or not from speech,
Each branch consists of a Convolutional Neural Network (CNN)
Spectrograms are visual representations of audio , which are computed by calculating the Short-Time Fourier Transform (STFT)  by cutting the audio into (not necessarily overlapping-) chunks and then computing the Discrete Fourier Transform (DFT)


DataBase:

was collected via the “COVID-19 sounds” Android app as well as through a web form The participants are asked to fill a survey about their demographic information (such as age and location), medical history, as well as symptoms (if any). The app instructed the participants to “breathe deeply five times, cough three times, and read three times a short sentence appearing on screen” 

survey Link
COVID-19 Sounds App survey





![Tux, the Linux mascot](https://ieeexplore.ieee.org/mediastore_new/IEEE/content/media/9474585/9474649/9474658/9474658-fig-1-source-large.gif)





APP SCREEN



Accuracy:
 It achieves an Unweighted Average Recall (UAR) of 74.9 %, or an Area Under ROC Curve (AUC) of 80.7% by ensembling neural networks. it achieves an Unweighted Average Recall (UAR) of 74.9 %, or an Area Under ROC Curve (AUC) of 80.7% by ensembling neural networks

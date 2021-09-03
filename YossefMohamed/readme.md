# Paper Link:

#### https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9474658

# Date of publish 
12 July 2021

# Classifications:

Recall COVID-19 positive (ACC+), also known as sensitivity, which is the true positive rate. 
Recall COVID-19 negative (ACC−), also known as specificity, which is the true negative rate.
Unweighted Average Recall (UAR): Also known as Unweighted Average Accuracy, is the average of sensitivity and specificity – the standard competition measure in the Interspeech ComParE challenge series. Chance level for two classes resembles 50.0 % UAR. 
Area Under ROC Curve (AUC): The ROC curve plots the true-positive rates against the false-positive rates with varying classification thresholds, and measures the area under the drawn curve. This measures how well a model can distinguish between the positive and negative classes, where a random baseline classifier will get a value of 50.0 %.
Accuracy (ACC): The ratio of examples that are answered correctly in the evaluation set.

# Features:
ImageNet Large Scale Visual Recognition Challenge (ILSVRC)
SVM models to classify if a person have COVID or not from speech,
Each branch consists of a Convolutional Neural Network (CNN)
Spectrograms are visual representations of audio , which are computed by calculating the Short-Time Fourier Transform (STFT)  by cutting the audio into (not necessarily overlapping-) chunks and then computing the Discrete Fourier Transform (DFT)

![Tux, the Linux mascot](https://ieeexplore.ieee.org/mediastore_new/IEEE/content/media/9474585/9474649/9474658/9474658-fig-1-source-large.gif)

# DataBase:

was collected via the “COVID-19 sounds” Android app as well as through a web form The participants are asked to fill a survey about their demographic information (such as age and location), medical history, as well as symptoms (if any). The app instructed the participants to “breathe deeply five times, cough three times, and read three times a short sentence appearing on screen” 

### survey Link
https://www.covid-19-sounds.org/en/app/

# Accuracy:
 It achieves an Unweighted Average Recall (UAR) of 74.9 %, or an Area Under ROC Curve (AUC) of 80.7% by ensembling neural networks. it achieves an Unweighted Average Recall (UAR) of 74.9 %, or an Area Under ROC Curve (AUC) of 80.7% by ensembling neural networks
 
 <hr />
 
 
# Paper Link:

https://arxiv.org/pdf/2009.08790.pdf

# Date of publish 
23 Sep 2020

# Classifications:

the pretrained weights from the cough non-cough pretraining task to initialize the model.
SGD is used as the optimizer, with an initial learning rate of 0.001 and decay of 0.95 after every 10 epochs
a batch size of 32 and train for a total of 110 epochs
Label smoothing is randomly applied between 0.1 and 0.3

# Features:
(1) Logistic Regression (LR) \n
(2) Gradient Boosting Trees \n
(3) Extreme Gradient Boosting (XGBoost) and \n
(4) Support Vector Machines (SVMs). As input to the classifiers,sarily overlapping-) chunks and then computing the Discrete Fourier Transform (DFT)\n
(5) Deep Convolutional Neural Networks (CNNs)\n


# DataBase:
## Non covid database
FreeSound Database 2018 (Fonseca et al. 2018)
Flusense (Al Hossain et al. 2020)
Coswara (Sharma et al. 2020)
## Covid database
data collection efforts have yielded a dataset of 3,621 individuals, of which 2,001 have tested positive.

# Accuracy:
AUC 0.72, t-test, p < 0.01, 95% CI 0.61—0.83


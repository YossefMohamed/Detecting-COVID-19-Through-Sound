# _DiCOVA Challenge: Dataset, task, and baseline system for COVID-19 diagnosis using acoustics_
### _Paper Link : https://arxiv.org/abs/2103.09148_

### _Basic Info_

- _**Publisher : Indian Institute of Science, Bangalore, ‡P. D. Hinduja Hospital**_
- **_Date : 17 Jun 2021_**

### _Architecture used_

1. _**Convolutional neural network (CNN)**_
2. **_CNN architecture based on ResNet18 with short-time magnitude spectrogram as input_**

### _Feature Extraction_

- **_MFCC_**
- **_`librosa `python library is used for the computation._** 

### _Model Training_

### _Note_
- **_The implementation uses the `scikit-learn ` python library._**
- **_DataSet Link: https://github.com/iiscleap/Coswara-Data_**

### _classification_

1. **_Logistic regression (LR)_**
2. **_Multi-layer perceptron (MLP)_**
3. **_Random Forest (RF)_**

### _The baseline system performance (Track 1 & 2)_
**_Track 1 
The goal is to use cough sound recordings from COVID-19 and
non-COVID-19 individuals for the task of COVID-19 detection._**

**_Cough_**  

- **_LR 66.95 (±1.74)_**
- **_MLP 68.54 (±1.65)_**
- **_RF 70.69 (±1.39)_**

**_Track 2
The goal is to use breathing, sustained phonation, and speech
sound recordings from COVID-19 and non-COVID-19 individuals for any kind of detailed analysis which can contribute towards COVID-19 detection._**

**_Breathing_**

- **_LR 60.95 (±2.17)_**
- **_MLP 72.47 (±1.96)_**
- **_RF 75.17 (±1.23)_**

**_Vowel_** 

- **_LR 71.48 (±0.55)_**
- **_MLP 70.39 (±1.84)_**
- **_RF 69.73 (±1.93)_**


**_Speech_** 

- **_LR 68.93 (±1.09)_**
- **_MLP 73.57 (±0.71)_**
- **_RF 69.61 (±1.56)_**

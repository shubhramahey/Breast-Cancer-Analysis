# Breast-Cancer-Analysis

The following project (Breast Cancer Analysis.ipynb) is on Breast Cancer where I created a predictive model to analyze the data to diagnose the Cancer as Malignant or Benign, as well as predict the variables that that influence breast cancer the most. The project focuses on covering data processing, descriptive analytics, EDA, visualization of data, applying Machine Learning techniques, increasing their accuracy to get the best model to predict the cancer data, Hyperparameter Tuning (Cross Validation), training models with the best predictors, ensemble the models, and making a Dashboard and final report about the results.

-----------------------------------------------------------------------------------

The Dashboard contains different sheets. 
(NOTE: Malignant(1) = TAR,i.e. target patients; Benign(0) = CTL, i.e. control patients; Test Data: 114 data points)

1) Confusion Matrix of the 3 main models I used for Cancer prediction namely, Random Forest, XGBoost, and Logistic Regression and their derived measures along with Accuracy and Precision. 

2) The probability Distribution of the Target and Control Patients by the 3 models with total of 43 patients that are classified as Malignant and 71 as Benign by the models.

3) Ensembler Tool: Setting about equal weights to all the 3 models used, since they all give about similar accuracy. This graph shows an ensembled probability distribution of the target and control patients, with their recall and precision calculated under the graph at the bottom.

4) The Raw Data has the imported patient ids; the actual class of the data/patient (Malignant, TAR or Benign, CTL); the data split (TEST/TRAIN, in this case TEST); the Probabilities and Class for all the 3 classifying models: RF (Random Forest), XGBoost, and LR (Logistic Regression); and the calculated/resulting Ensembled Score and ensembled class (Malignant/Benign) for the Test set patient data.

5) Ensemble Summary shows the Precision-Recall trade-off for the data. I came to an optimal number of patients (which usually depends on the client, if they want more number of patients and sacrifice on the recall/precision, or need a balanced precision-recall as well as patient counts). Here, I selected 40 patients with probability threshold >=70% for classifying the data as M or B, and with a recall of 93% and a 100% precision (which is highly ideal, but the model was well-trained and data cleaned properly).

6) ROC curves, Area Under the Curve (AUC) and Precision-Recall curves for all the 3 models, i.e. Random Forest, XGBoost and Logistic Regression.

7) Variable Importance shows the importance of all the variables with their MDI (Mean Decrease Impurity) from the code, along with their variable descriptions. When sorted, the top variables come out to be: area_mean, area_se, concavity_mean, symmetry_worst, texture_mean, smoothness_worst, and fractal_dimension_se (from both XGBoost and Random Forest, as shown in the python code).


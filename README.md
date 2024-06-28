# Cancer Detection/Diagnosis Model Comparison
## Project Overview
This project aims to compare the performance of various machine learning models in detecting and diagnosing different types of cancer based on gene expression data. The types of cancer analyzed include Breast, Colon, GBM (Glioblastoma), and Lung cancer. The models compared in this project are Random Forest, Support Vector Machine (SVM), and Neural Network (MLP).
##Data Acquisition
Gene expression data for various cancer types is obtained from a publicly available dataset. The data is downloaded and extracted programmatically using the requests and zipfile libraries.

## Data Preprocessing
**Loading Data:** Gene expression data for Breast, Colon, GBM, and Lung cancers is loaded from text files into pandas DataFrames.
**Filtering Common Genes:** Only genes common to all four types of cancer are retained for analysis.
**Combining Data:** Gene expression data is combined into a single DataFrame, with an additional column indicating the type of cancer.
**Splitting Data:** The combined data is split into training and testing sets.
**Scaling Data:** Feature scaling is performed using StandardScaler.

## Model Training and Evaluation
Three machine learning models are trained and evaluated:

**Random Forest:**
A Random Forest Classifier is trained on the gene expression data.
Model accuracy is evaluated on the test set.
**Support Vector Machine (SVM):**
An SVM with a linear kernel is trained on the scaled data.
Model accuracy is evaluated on the test set.
**Neural Network (MLP):**
A Multi-Layer Perceptron (MLP) classifier is trained on the scaled data.
Model accuracy is evaluated on the test set.
Performance metrics such as precision, recall, and F1-score are calculated for each model.

## Results
The accuracy of each model is printed, and a comparison of their performance metrics is visualized using a bar plot.

- Random Forest Accuracy: rf_accuracy
SVM Accuracy: svm_accuracy
Neural Network Accuracy: nn_accuracy
Performance metrics for precision, recall, and F1-score are plotted for each model.

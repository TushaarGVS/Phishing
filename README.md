# Feature Selection for Spam and Phishing Detection

The ease of communicating through email saw a huge increase in Unsolicited Bulk Email(UBE). Unsolicited emails are broadly divided into 2 categories: Spam(mass mailing approach to marketing) and Phishing(impersonatisation for the purpose of stealing data). 
This project gives a machine learning to approach to classify them into spam and phishing categories. It considers a total of 40 features which are broadly categorised into URL based, body based, sender based, subject based and script based features. 

An addition to this extraction involved _feature selection_ using:
* Low Variance filter
* High correlation filter
* Feature importances
* **mRMR**

## Getting Started

The project has been divided into 3 modules for convenience. 
The first module deals with extraction of intricate features from the emails and preparing the dataset for application fo the module.
The entire procedure is illustrated as below! 

### Requirements

* Python2
* Jupyter Notebook
* Necessary Python libraries (check first cells of [Feature Extraction](https://github.com/TushaarGVS/Phishing/blob/master/code/feature_extraction.ipynb) and [Feature Selection](https://github.com/TushaarGVS/Phishing/blob/master/code/feature_selection.ipynb))

### Running
* Run [Feature Extraction](https://github.com/TushaarGVS/Phishing/blob/master/code/feature_extraction.ipynb) sequentially to obtain 3 datasets in CSV format
* Once CSVs with 40 features have been generated, now run the [Feature Selection](https://github.com/TushaarGVS/Phishing/blob/master/code/feature_selection.ipynb) sequentially
* In [Feature Selection](https://github.com/TushaarGVS/Phishing/blob/master/code/feature_selection.ipynb), the reference file chosen was ```dataset_HSP.csv``` which can be changed in the calling of ```mRMR_CSV('dataset_HSP', 'label')```

### Testing and Results
```Voting Ensemble classifier``` with SVM, Naive Bayes, LDA, Adaboost, Random Forest and CART was used in the implementation of mRMR feature selection
The selected feature accuracy was tested against the origibal (40 features) using the following algorithms:
* Voting Ensemble classifier (same as above)
* SVM
* Stochastic Gradient Boosting
* Extra Trees classifier
* Adaboost
* Random Forest
* Bagged Decision Tree classifier (CART)
* Naive Bayes

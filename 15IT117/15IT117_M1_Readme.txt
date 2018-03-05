Project title: Feature Selection for Spam and Phishing Detection

Description: The ease of communicating through email saw a huge increase in Unsolicited Bulk Email(UBE). Unsolicited emails are broadly divided into 2 categories: Spam(mass mailing approach to marketing) and Phishing(impersonatisation for the purpose of stealing data). This project gives a machine learning to approach to classify them into spam and phishing categories. It considers a total of 40 features which are broadly categorised into URL based, body based, sender based, subject based and script based features. A decision tree model is used for the purpose of classification in Python.

The project has been divided into 3 modules for convenience. The first module deals with extraction of intricate features from the emails and preparing the dataset for application fo the module.

Requirements:
- Python2

Getting Started:
1.The following Python libraries need to be installed for making the source code file work:
- re
- BeautifulSoup
- urlparse
- email
- os
- HTMLparser
- IPy

2. Running the Project
- Install Jupyter Notebook.
- Run the code in sequential order (module-wise) using the command:
	jupyter notebook 15IT117_M1_feature_extraction.ipynb

3. Files enclosed in the folder (15IT117)
- 15IT117_M1_Readme.txt
	Detailed description of all the files uploaded and the dependencies
- 15IT117_M1_feature_extraction.ipynb
	The iPython notebook file that contains entire Python code to extract features and form datasets
- 15IT117_M1_test
	Contains 5 test cases (test1.eml, test2.eml, test3.eml, test4.eml, test5.eml)
- 15IT117_M1_test.csv
	The extracted dataset from the test files, with class label as '?'
- 15IT117_M1_screenshots
	Contains 5 screenshots of corresponding processing of test files (format: test[test_number]_screenshot.png
 
The source code is well commented so one can easily understand the motive behind each and every step.

Testing:
The path of the test file has been specified in the source code file itself. The user can alter this to suit the specifications of his running environment. The given test cases are simple and were used for validation of the code which can be cross verified.

1. Test Data Description
There are a total of 5 test files each of which have a few specific features set. These will test whether the features are being correctly extracted from an email.

Authors:
Nihar Raichada 15IT132
Tushaar Gangarapu 15IT117

Acknowledgments:
We would like to thank Dr. Jaidhar CD and Mr. Ganesh Murgod for encouraging us and guiding us during the implementation of this project.

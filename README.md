# Capstone Project:
# A method of detecting AI generated text
# Data:
This dataset comes from the Kaggle Machine Learning repository. The student data is collected from students and AI generated text is from chatgpt.

# Data Cleanup
This dataset has 1103 rows and 2 columns containing 'Text' and 'Label'. The column 'Text' is the feature and the column 'Label' is the target variable. There is a missing entry in the dataset so we have to address this issue before starting data analytics.

# Data Analytics
The dataset contains words and sentences in English. Text data needs to be processed and converted them into vectors. We build and compare four classifier models. By using GridSearchCV and tuning hyper parameters, we can find the best model. 

# Findings
- The dataset is balanced becuase it has 50% in class 0 and 50% in class 1
- A pipeline combining CountVectorizer and classifier is able to detect AI generated text
- SupportVectorMachine model achieves the accuracy score 0.99 with non-linear kernel
- With GridSearchCV, we find the best CountVectorizer hyperparameters are max_features=750 and stop_words=None


# Summary
Supervised learning is one of the most useful machine learning technology to solve binary classification and mutli-class classification problems. We proposed a method to detect AI generated text by building and comparing four classifier models: LogisticRegression, DecisionTree, NaiveBayes and SupportVectorMachine. SupportVectorMachine is the best classifier among all because it achieves higher scoring with non-linear kernels. I would like to deploy this model to my web server and continue to optimize model performance by collecting more AI generated text and applying other machine learning technique such as Ensemble model and Neural Network. I hope this can be useful and turned into a good business tool.
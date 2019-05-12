AIT 690 Project Natural Language Processing
Team name : A team has no name
Members: Vidhyasri, Rahul Pandey, Arjun Mudumbi Srinivasan

This python script is used to develop the base model of the sarcasm/irony detection. We start with importing the necessary libraries , reading the data
from the text file, followed by splitting the data into columns and making a dataframe. The data is cleaned using few functions which involves removing the mentions
urls and others . Bag of words model is developed using the Sklearn's TFIDF vectorizer.
data is split into train and test and the models like svm , decision tree is used to predict. The accuracy and F-1 scores are determined using sklearn implementation

File Usage :
$ python baseline-approach.py training_file_path test_file_path
where:
        training_file_path: Can be SemEval2018-T3-train-taskA_emoji.txt or SemEval2018-T3-train-taskB_emoji.txt. Depending on whether task A or task B is being performed
        test_file_path: Can be SemEval2018-T3-test-taskA_emoji.txt or SemEval2018-T3-test-taskB_emoji.txt. Depending on whether task A or task B is being performed

Output: Accuracy and F-1 scores of different models and confusion matrix of the best performing baseline model i.e. SVM

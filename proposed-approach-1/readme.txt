AIT 690 Project Natural Language Processing
Team name : A team has no name
Members: Vidhyasri, Rahul Pandey, Arjun Mudumbi Srinivasan

This python script is used to develop the first proposed approach model of the sarcasm/irony detection. We start with importing the necessary libraries , reading the data
from the text file, followed by splitting the data into columns and making a dataframe. The data is cleaned using few new functions compared to base model which involves removing the mentions
urls and others, expanding hashtags(#IAmJoking -> i am joking), contraction words ("There's -> there is"), etc..

We created the average of word embeddings as features. We used GloVe vectors and Google's word2vec as embedding features
Data is split into train and test and the models like svm , decision tree is used to predict. The accuracy and F-1 scores are determined using sklearn implementation

File Usage :
$ python proposed-approach-1.py training_file_path test_file_path embedding_type embedding_path
where:
        training_file_path: Can be SemEval2018-T3-train-taskA_emoji.txt or SemEval2018-T3-train-taskB_emoji.txt. Depending on whether task A or task B is being performed
        test_file_path: Can be SemEval2018-T3-test-taskA_emoji.txt or SemEval2018-T3-test-taskB_emoji.txt. Depending on whether task A or task B is being performed
        embedding_type: glove/word2vec any of the one
        embedding_path: File path of the embedding file (GloVe/Word2vec)

Output: Accuracy and F-1 scores of different models and confusion matrix of the best performing baseline model

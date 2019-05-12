AIT 690 Project Natural Language Processing
Team name : A team has no name
Members: Vidhyasri, Rahul Pandey, Arjun Mudumbi Srinivasan

This python script is built on top of this Github Code:
https://github.com/dennybritz/cnn-text-classification-tf
which implements Kim's CNN for sentence classification (https://arxiv.org/abs/1408.5882)

This code trains a CNN network of 3 parrallel convolution-maxpool layer of filter size 3,4,5 respectively. Followed by
one fully connected layer, dropout layer of 50% dropout, and finally a softmax layer.
It Uses Adam Optimizer for optimization and cross entropy function as loss function.

It also uses data_helper.py file to clean and load the data and also split the data into batches
The config.yml file contains information about word2vec path, glove path, etc.

File Usage :
$ python train.py training_file_path

Note: Please update the config.yml for local path of the embeddings

where:
        training_file_path: Can be SemEval2018-T3-train-taskA_emoji.txt or SemEval2018-T3-train-taskB_emoji.txt. Depending on whether task A or task B is being performed

Output: Trained weight stored in runs folder in the current directory, which stores the weights at different checkpoints

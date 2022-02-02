# README
Follow the following instructions while running the colab notebook.
1) First mount the google drive.
2) After that we open the saved pickle file of the dataframe (which is a preprocessed
dataset) from the drive. The link of the dataset (dataframe) is given below -
https://drive.google.com/file/d/19C7rZBt-uiM2IiJRiAGqnAZor299hXbO/view?usp=sharing

3)Then we import libraries like numpy,pandas,json etc.
4)Now we install top2vec model by using the command: pip install top2vec

5)Then we train top2vec model on cord-19 dataset and use top2vec model as :- top2vec
= Top2Vec(documents=df2.abstract, speed="learn", workers=4)
Here top2vec takes some important parameters like documents,speed and workers.
Documents:- it is defined as an input corpus which is in the form of a list of strings.
Speed:- speed parameter defines how fast the model takes to train. The 'learn' option will
learn better quality vectors but take a longer time to train.
Workers:- It defines the amount of worker threads to be used in training the model.

6) we find different values like topic number,topics etc.
7) We also generate word clouds
8)After that we find answers to queries using the model.
9) We also find similar words for keywords.
10) when the query gives to the model,it extracts keywords and finds clusters then
returns the abstract of the best document searched.
11) Then we run the model on a list of questions to generate an answer for them and
compare with the actual answer we find blue score,precision,recall and f1-score.

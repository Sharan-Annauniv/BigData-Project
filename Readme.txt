# Hate-Speech-Detection

This project is an attempt to write a text classifier that can automatically detect hate speech, 
which will have potential applications in forum moderation and filtering on social media feeds. 


# Contents

*Dataset:* This folder contains the XML files containing the text corpus. The text in this corpus was collected from Twitter, and was annotated using [MAE](http://keighrim.github.io/mae-annotation/). Each file contains a set of tweets, along with XML tags representing annotations. \[*CONTENT WARNING:* Because the goal of this project is to train an algorithm to identify and filter out hate speech, the text corpus contains many examples of said hate speech, including racism, sexism, ableism, homophobia, transphobia, anti-immigrant rhetoric, body-shaming, religious intolerance, and other general nastiness. *Caveat lector.*\]

*HS_classifer.py:* A Python program to extract the data from the files in the GoldStandards folder and use it to train and test two naive Bayesian classifiers. The first is a simple classifier that uses as features all of the words in the text; this is meant to serve as a baseline against which other classifiers can be evaluated. The second classifier uses the annotations to determine which words should be considered as features.


#Run
Execute the command python hs_classifier.py in the cmd (python2 version),
The accuracy of the training data and the test data will be returned by the classifier.
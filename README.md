A Sentiment Analysis Research Project:

As the final project for the Fall 2022, Intro to Python course at the Hertie School, our team compared various NLP models to determine the accuracy and f1-score of said models. 
To rank these models we ran comparisons on an aggregated data set collected via polling our friends and families on questions concerning wedding RSVPs - Data hyplerlinked HERE

Background:

Planning a wedding is highly challenging and costs a lot of time. To make the planning process a bit easier for couples, we wanted to have a sentiment analyzer in place to automatically analyze the responses to wedding invitations. For this, we made a research project to test five different pre-trained analyzers on a testing set with responses to wedding invitations and check their accuracy. This research project strives to answer the question: Which is the best Sentiment Analyzer Tool to analyze wedding invitation responses?

Process:


Collect Data: Asking friends about responses to a wedding invitation​
Analyzing the responses by using five sentiment analyzers​
Input: all responses​
Output: “pos” / “neg”​
Comparing the results to the true situation by using measurement tools​
Getting the best sentiment analysis tool for our purpose

Our script had a total of six functions; 5 NLP models for sentiment andalysis and one function for accuracy and an F1 score. 

How to Run:

The file sentiment analysis in the intro2python folder contains the script necessary to run the application. Functions needed to run the file are saved in and imported. The functions, and applications necessary for download are as follows;

Sentiment Analyzers: 
HappyTransformer,
Flair_Analysis,
HuggingFace_Bertweet,
TextBlob_Analysis,
Vadar_Analysis, 

Import:  
pandas,
Openpyxl,
TextClassifier,
NLTK_data - Vadar_Lexicon,
Senten,
Split_Single,
HappyTextClassificiation, 
F1_score,
Accuracy Score,



Possible future improvements and extensions:


Collecting more data, and working towards tuning the model would aid further in ranking the NLP models an exciting extension to this project would be an API that could run sentiment analysis on emails. 

Authors:
Anna Morhon, Irene Quadrelli, Maurice Rios


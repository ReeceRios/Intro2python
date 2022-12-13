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
The desired results are produced in an excel table, this is availbel two download with two sheets: one that gives the full sentiment analysis table, one sheet with the accuracy scores

Our script had a total of six functions; 5 NLP models for sentiment andalysis and one function for accuracy and an F1 score. 

How to Run:

The file sentiment analysis in the intro2python folder contains the script necessary to run the application. Functions needed to run the file are saved and imported. The functions, and applications necessary for download are as follows;

Results:

![image](https://user-images.githubusercontent.com/113826312/207464990-6ba90197-ec54-4513-8763-5129841ccc25.png)


Sentiment Analyzers: 

HappyTransformer,  is an package built on top of Hugging Face's transformer library that makes it easy to utilize state-of-the-art NLP models
#pip install transformers flair happytransformer
Flair_Analysis, allows you to apply our state-of-the-art natural language processing (NLP) models to your text, such as named entity recognition (NER), part-of-speech tagging (PoS), special support for biomedical data, sense disambiguation and classification, with support for a rapidly growing number of languages.
HuggingFace_Bertweet, BERTweet is the first public large-scale language model pre-trained for English Tweets. BERTweet is trained based on the RoBERTa pre-training procedure. The corpus used to pre-train BERTweet consists of 850M English Tweets (16B word tokens ~ 80GB)
TextBlob_Analysis, extblob is a Python NLP library that uses a natural language toolkit (NLTK). It uses NLTK because it is simple, easy to deploy, will use up fewer resources, gives dependency parsing, and can be used even for small applications
Vadar_Analysis,( Valence Aware Dictionary for Sentiment Reasoning) is a model used for text sentiment analysis that is sensitive to both polarity (positive/negative) and intensity (strength) of emotion. It is available in the NLTK package and can be applied directly to unlabeled text data.

Import: 

    pandas,import pandas as pd 

    import pandas as pd
    from transformers import pipeline

    import pandas as pd
    import openpyxl
    
    import flair
    from flair.models import TextClassifier
    from flair.data import Sentence
    from segtok.segmenter import split_single
    
    from textblob import TextBlob
    
    from happytransformer import HappyTextClassification
    
       import nltk 
    import pandas as pd
    nltk.download("vader_lexicon") 
    
    from sklearn.metrics import f1_score, accuracy_score
    from xlsxwriter import Workbook

Possible future improvements and extensions:

Collecting more data, and working towards tuning the model would aid further in ranking the NLP models an exciting extension to this project would be an API that could run sentiment analysis on emails. 

Authors:

Anna Morhon, Irene Quadrelli, Maurice Rios


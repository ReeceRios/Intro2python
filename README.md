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

<img src="https://user-images.githubusercontent.com/113826312/207464990-6ba90197-ec54-4513-8763-5129841ccc25.png" width="150" height="100">

Sentiment Analyzers: 

* HappyTransformer: a package built on top of Hugging Face's transformer library that makes it easy to utilize state-of-the-art NLP models. 
* Flair: also based on Hugging Face. Trained on IMDB movie reviews dataset, features include: named entity recognition (NER), part-of-speech tagging (PoS), special support for biomedical data, sense disambiguation and classification, with support for a rapidly growing number of languages.
* Hugging Face: also trained on Twitter data. The Hugging Face hub has hundreds of different sentiment analysis tools and datasets available. 
* TextBlob: TextBlob is a Python NLP library that uses NLTK and the Pattern libraries. Features include: part-of-speech tagging, classification, translation and more. 
* Vader (Valence Aware Dictionary for Sentiment Reasoning): trained on Twitter/social media data. It is sensitive to both the intensity and polarity of sentiment. 

Install: 

#pip install transformers flair happytransformer xlsxwriter 

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

Anna Mohn, Irene Quadrelli, Maurice Rios


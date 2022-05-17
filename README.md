![giphy (1)](https://user-images.githubusercontent.com/57909909/168902321-760c3caf-864f-4f2c-b5ee-6199863df92f.gif)

# Tweet Sentiment Extraction
## Introduction

Sentiment analysis (or opinion mining) is a natural language processing technique used to determine whether data is positive, negative or neutral. Labels of positive, negative or neutral are contextual and subjective.

This is a quite unique project for me . As , here I need to extract phrase from a sentence base on some sentiment .
This case study is about capturing extracted support phrases from given text based on sentiment. This is one of the Kaggle problems named Twitter Sentiment Extraction.

## Business problem
With all of the tweets circulating every second it is hard to tell whether the sentiment behind a specific tweet will impact a company or a person's brand for being viral (positive) or devastate profit because it strikes a negative tone. Capturing sentiment in language is important in these times where decisions and reactions are created and updated in seconds. But which words actually lead to the sentiment description? In this problem we need to pick out the part of the tweet (word or phrase) that reflects the sentiment .

Example

text : "Sooo SAD I will miss you here in San Diego!!!"
sentiment : negative
selected_text: "Sooo SAD

## ML formulation of the business problem

Given a text and the sentiment we have to predict the selected text (which is the a word or phrase of the text).
- Here is a tweet : " my boss is bullying me…"
- sentiment of the tweet is : "negative"
- Words defining that it is a negative tweet : "bullying me" (this is something we want to find in this case study).
Answer such questions like what kind of problem is it (classification regression)? - This is a little bit difficult to answer but i would say it is a classification task but in a different way (because we have to classify the phrase of the text associated with sentiment).

# Model i used 
- LSTM
- Bi-LSTM
- Roberta
Finally i choose Roberta because its giving good jaccard score but in real world we will consider application  latency and model shold not be more expensive in terrms of ram ,excution etc.
# Roberta architecture

![1_EMgwYCOaps6iSahu_l_Atg](https://user-images.githubusercontent.com/57909909/168904195-85d43768-1e1d-4ec9-8a9f-ac4b860ff931.png)



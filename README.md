# Natural_Language_Processing

![nlp](https://user-images.githubusercontent.com/55191934/77843737-c10f8980-71bd-11ea-8dd0-6ecf87194879.jpg)


This repository aims to delineate Natural Language Processing techniques through a succint Python codes.

The package to be used is 'SCRAPY', from which the English language model can be loaded as 'en'. Other
language models also can be installed from scrapy. 

nlp = spacy.load('en') stores functions in nlp wherein it acts a pipeline.

This repository features a WORD USAGE CLASSIFIER which helps to classify whether the sentence(document) belongs 
to the 'animal' class or the 'language' class for the WORD Python. Since it can be inferred as the animal or the 
language too, hence a classifier is made. 

THe workflow of this classifier is as shwn below:

![WhatsApp Image 2020-03-31 at 4 43 34 PM](https://user-images.githubusercontent.com/55191934/78020839-ca405800-736f-11ea-8795-b0404ed7fa85.jpeg)

The main components of this pipeline are:

(a) Bag of Words model

(b) Term-Frequency Inverse_Document_Frequency

(c) Prediction (using the Naive Bayes MultinomialNB)

Bag of Words model is based on the CountVectorizer which converts the words into a sparse matrix containing each word with it's index.
This count now contains many words such as 'the', 'or', 'and' which occur very frequently but do not contribute to analysis. These 
are called STOP WORDS.

The TF-IDF thereby gives weightage to the words in the count matrix. 

Learnings:

1. Model improved slightly on using n=2 instead of n=1 in n grams model.

2. The working of TF-IDF.

Results:

![nlp2](https://user-images.githubusercontent.com/55191934/78021568-18099000-7371-11ea-9933-cd5b8c954318.PNG)

This is how the prediction looks:

![nlp1](https://user-images.githubusercontent.com/55191934/78021660-3ff8f380-7371-11ea-97fc-eebafa95e83e.PNG)

There have been some mis classifications. The way it is trained to work is that: It identifies main important words which characterize
it into a label(animal/language) such as bites, venom(animal) in contrast to bytes, memory(language)

The working of this is really fascinating!

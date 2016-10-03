nextWordPredict
======================================================== 
font-family: 'verdana'
transition: rotate
author: Pradeep K. Pant, ppant@cpan.org
date: October 3, 2016


        Coursera / Johns Hopkins University 
          Data Science Specialization
           Switftkey Capstone Project 

Building a predictive text model
========================================================

- Create an algorithm for predicting the next word given one or more words as input using NLP

- A large corpus of blog, news and twitter data was loaded and analyzed. 

- N-grams were extracted from the corpus and then used for building the predictive model. 

- Various methods of improving the prediction accuracy and speed were explored.

Algorithm 
========================================================

- N-gram model with stupid back-off strategy was used

- Dataset was cleaned, lower-cased, removing links, twitter handles, punctuations, numbers and extra whitespaces, etc

- Matrices from 6-gram to uni-gram were extracted using RWeka 

- Reduced size of model by dropping least frequent N-grams

Shiny App interface
========================================================

- Provides a text input box for user to type a word/phrase

- Detects words typed and predicts the next word reactively

- Iterates from longest N-gram (6-gram) to shortest (2-gram)

- Predicts using the longest, most frequent, matching N-gram

- Option to select no, of prediction displayed

App and resources
========================================================

- Average response time under 2-3 seconds

- Application memory usage well under 200MB

- Application is running at: https://ppant.shinyapps.io/nextWordPredict

- Github link for various code files is here: https://github.com/ppant/Coursera-Data-Science-Capstone-Project. 

In future, Code will be updated with any new features/improvements.

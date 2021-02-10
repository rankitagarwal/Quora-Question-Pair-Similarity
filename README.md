# Quora-question-pair-similarity
## Business Problem
### Description

Quora is a place to gain and share knowledge—about anything. It’s a platform to ask questions and connect with people who contribute unique insights and quality answers. This empowers people to learn from each other and to better understand the world.

Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.

    Credits: Kaggle

### Problem Statement

    Identify which questions asked on Quora are duplicates of questions that have already been asked.
    This could be useful to instantly provide answers to questions that have already been answered.
    We are tasked with predicting whether a pair of questions are duplicates or not.

### 1.3 Real world/Business Objectives and Constraints

    The cost of a mis-classification can be very high.
    You would want a probability of a pair of questions to be duplicates so that you can choose any threshold of choice.
    No strict latency concerns.
    Interpretability is partially important.

# Machine Learning Probelm
##  Data
###  Data Overview

- Data will be in a file Train.csv
- Train.csv contains 5 columns : qid1, qid2, question1, question2, is_duplicate
- Size of Train.csv - 60MB
- Number of rows in Train.csv = 404,290
###  Example Data point

"id","qid1","qid2","question1","question2","is_duplicate"
"0","1","2","What is the step by step guide to invest in share market in india?","What is the step by step guide to invest in share market?","0"
"1","3","4","What is the story of Kohinoor (Koh-i-Noor) Diamond?","What would happen if the Indian government stole the Kohinoor (Koh-i-Noor) diamond back?","0"
"7","15","16","How can I be a good geologist?","What should I do to be a great geologist?","1"
"11","23","24","How do I read and find my YouTube comments?","How can I see all my Youtube comments?","1"

##  Mapping the real world problem to an ML problem
###  Type of Machine Leaning Problem

It is a binary classification problem, for a given pair of questions we need to predict if they are duplicate or not.
### Performance Metric
- Log loss and confustion matrics




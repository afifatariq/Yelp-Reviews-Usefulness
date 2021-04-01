# Yelp Reviews Usefulness

## Abstract  
Abstract—Reviews analysis is a challenging machine learning task due to the recursive nature of sentences in the reviews.  Traditional approaches to review analysis use count or frequency of words in the text which are assigned a value of  usefulness. These approaches disregard the order of words and the complex meanings they can convey. Gated Recurrent  Units (GRU) and Long Short Term Memory (LSTM) are a type of recurrent neural networks which have the ability to  store information of long term dependencies in sequential data. In this paper, I have compared both GRU and LSTM  models for analyzing the usefulness of reviews.  

## Introduction  
The internet has brought all things to our fingertips, from buying groceries to researching about the best restaurants in  the area. It has become a place where consumers evaluate products and services based on impressions and feedback from other  consumers. In 2017, customers read an average of seven reviews before trusting a business. Thus, the importance of showing the users the most useful reviews at the top of the page is very beneficial.  

Yelp as stated on their website is a popular online directory for discovering local businesses ranging from restaurants,  and cafes to hairdressers, spas, and gas stations. The number of reviews posted every minute by yelp users is 26,380. This  amount shows the extent of popularity of writing and reading reviews.  

In my work, I have focused on finding the usefulness of reviews posted. Not all the reviews posted are actually  beneficial for people who want to know what a business is like. Some reviews are very thorough and detailed where as some just state whether they had a good experience or bad without mentioning the reason. These reviews have been voted as useful or not  by the other yelpers. I will be using this data to train my neural network to predict whether a review would be useful or not.  

The neural networks that I will be using are a type of recurrent neural network (RNN); Gated Recurrent Units (GRU)  and Long Short Term Memory (LSTM). RNN’s are neural networks that are good at modeling sequence data. An RNN has a  looping mechanism that allows information to flow from one step to the next. As the RNN processes more steps, it has trouble  retaining information from previous steps. This is the vanishing gradient problem in the traditional RNNs. For reviews, we have  very long sequence of textual data so this problem is unavoidable which is why I will be using GRU and LSTM which take care  of the vanishing gradient problem.  

I will be using the same input data and labels for both models. I will then be applying the same preprocessing  techniques meaning the cleaning of text, embedding, and converting to integers. After doing these pre-processing techniques, I will input my training data into my GRU or LSTM model. Both of these models give me a different accuracy based on their  performance.  

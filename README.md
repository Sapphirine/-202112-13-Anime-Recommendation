# Sapphirine Anime Recommendation
Columbia EECS6893 final project 2021Fall team13

### Team member:Zijun Wei, Hanwei Tang, Yifan Wang

Project Name: Anime Recommedation

Youtube Video Link:https://youtu.be/7NbISkU3ayg

## Desicription
This repository contains the work for the final project for EECS E6893 - Big Data Analytics taught by Prof. Ching-Yung Lin.

## Dataset
All the data are scrapped from www.animelist.com using Jikan API.

Jikan Api:https://jikan.docs.apiary.io/#introduction

## Methodology
Machine Learning Alogorithms: Linear Regression, Random Forest, Decision tree, Gradient boosted tree, KNN

Deep Learning Algorithmns: DLRM

Modules: Tensorflow, Keras, Sklearn, Pyspark

## Introduction of Project

Anime usually refers to animation produced in Japan. The anime industry has been developed quickly since last century, watching anime has been a popular choice for people of all ages in the whole world. Although some titles are loved by nearly everyone, most anime can only attract limited amount of audience. Everyone has different taste on anime, finding the suitable anime to watch is important and sometimes difficult for anime fans. To solve this problem, we developed an anime recommendation system. We decided to pick up our data from myanimelist.com.

Our main goal is to make anime recommendation for users, and we provide two different choices. The first is to make content-based prediction for the general score of each anime and KNN prediction for similar animes to picked anime. Four different models, including Linear Regression, Random Forest, Decision Trees and Gradient-Boosted Trees, are achieved and compared in this part. The Linear Regression model results in best accuracy with 83% according to our test. And we construct a KNN model to find similar anime to the specific anime. The other choice is to make personalized recommendation based on Collaborative Filtering, by looking for users who share the same rating patterns with the target user and make prediction based on what these similar users like. In this part, we used neural network of deep learning method to train the model and predict users’ personal ratings for each anime. And the best neural network model we got has 48.93% accuracy.


## Organization of the directories
```
./
├── Collaborative algo
│   ├── CF Algo recommendation for Deep learning model after adding more metadata.ipynb
│   ├── Neural network model train.ipynb
│   └── recommendation-system-cf-anime for simple NN structure.ipynb
├── Content-based algo
│   ├── Using sklearn buildup KNN model.ipynb
│   └── pyspark content-based flitering.ipynb
├── README.md
├── Result graphs and model structures
│   ├── complex NN model accuracy.png
│   ├── complex NN model loss.png
│   ├── complex NN model setup.png
│   ├── linear NN model loss.png
│   ├── linear NN model setup.png
│   ├── meta NN model accuracy.png
│   ├── meta NN model loss.png
│   ├── meta NN model setup.png
│   └── 数据截图.docx
└── data scrapping
    └── All Scrapping process.ipynb

4 directories, 16 files
```

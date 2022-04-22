# Tanzanian Water Wells
## Phase 3 Project
### Author
- Jordan Kominsky: 
[LinkedIn](https://www.linkedin.com/in/jordan-kominsky/) | 
[GitHub](https://github.com/jskominsky) | 
[Email](mailto:jskominsky@gmail.com)

![8a447806-33a1-4f65-aff9-fe4a790768c1](https://user-images.githubusercontent.com/100230332/164601615-ea646516-98e6-4d53-995d-525eb970f4f7.jpeg)

## Overview
In Tanzania, 4 million people lack access to safe water according to [water.org](https://water.org/our-impact/where-we-work/tanzania/#:~:text=4%20million%20people%20in%20Tanzania,long%20distances%20to%20collect%20water.).  They mainly rely on water wells for access to clean drinking water, however many of the water wells in Tanzania are not functional.  My goal is to build a predictive model, using classification models, for the charity, The Tanzania Water Project, to predict whether a water well is functional or non functional.

![1700-1536x960](https://user-images.githubusercontent.com/100230332/164609235-dd4eb5f6-13d4-452f-9c42-8086a0957944.jpg)

## Problem
Nearly 50% of the water wells in Tanzania are non functional, according to the data I was provided. This is a major waste of both money and resources.  I built a predictive model for the Tanzania Water Project, a charity who is helping build water wells throughout the country.  By being able to predict which water wells are non functional and need to be rebuilt or repaired, I can help the charity properly allocate their precious resources.

![tanzania-mount-kilimanjaro](https://user-images.githubusercontent.com/100230332/164615946-3aea9aef-8fcf-48c1-bd41-5138e1e65b6b.jpeg)

## Data
My data was found on drivendata.com and has nearly 60,000 data points regarding water wells in Tanzania.  The data included whether or not a well was functional or non functional. 

![functional_bar](https://user-images.githubusercontent.com/100230332/164612880-99a5705d-f86d-4f0f-960e-ac591d36dfdc.jpeg)

## Methods
I used a variety of different classification models to improve the ability of the model to predict whether a water wall was functional or non functional. I started off with a Dummy Classifier to help establish a baseline to compare all future models against. After this I tried a variety of different algorithms hypertuning them where I felt necessary. The specific methods used are:
- Logistic Regression
- Logistic Regression with GridSearch to tune hyper parameters
- Random Forest Classifier
- XGBoost Random Forest Classifer  
- XGBoost Random Forest Classifer with GridSearch to tune hyper parameters

My best performing model was my XGBoost Classifier with default values, which had an accuracy of 86% on my training data, and an accuracy 84.9% on my training data, when predicting functional or non functional. The accuracy for just 'functional' status was 75.39% and the accuracy for just ' non functional' status was 93.99%

### XGBoost Confusion Matrix on Training Data

<img width="337" alt="Confusion Matrix" src="https://user-images.githubusercontent.com/100230332/164613799-d6e0a7a0-f7a6-4ee8-a157-070eef0a944d.png">

### XGBoost Confusion Matrix on Testing Data

<img width="337" alt="Confusion Matrix Test Data" src="https://user-images.githubusercontent.com/100230332/164761930-780e3ed2-7f26-4562-bbd2-8fbb184c8db7.png>



## Next Steps

![1_8qTfnlqpcU-TSZ3MsN1zAA](https://user-images.githubusercontent.com/100230332/164614263-d33bc7e8-b8b4-4fe8-ac90-26df68641b5c.jpg)

Given more time I would like to use a time series analysis to better predict when functional wells will begin to break down and need repair.  I would also like to develop an application that allows the charity to plug in the specifications of wells they are considering buildng (ie location, waterpoint type, water quality, etc) and get an instant prediction about if the well will be functional or not and how long they can expect the well to remain functional.  This will help the charity properly allocate their resources.

## Repository Structure

```
 ├── Data
 ├── Images
 ├── Pickles
 ├── gitignore
 ├── Final_Notebook.ipynb
 ├── Tanzanian Water Wells.pdf
 └── README.md
 ├──LICENCE
```

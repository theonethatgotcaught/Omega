# Real or Not? NLP with Disaster Tweets
## Team Omega
Maxime Dubi

Kamila Mananova

Bleron Ramaj

## 📑Project description 
Real or Not? NLP with Disaster Tweets: For this project we are challenged to buil a Machine Learning model that can predict which tweets are about a real disaster (1) and which are not (0). 

## 📊 Data 
There is two datasets:

  df_train where we have 6471 rows and five columns.
  
  df_test with 1142 rows where we have to applied our models to predict the "target" column
  
## 🎯 Project structure
**Preparation**

Create new GitHub repository

Create python notebook with Colab

We did an EDA to see what we need to preprocessing

  Merged the keywords with the text
  
  
  Clean the data
  
     Delete the links
    
     Upper case to lower case
    
     Delete unnecessary symbols: @, #,...
    
    
    
  Tokenizer (spacy tokenizer )
  
     Lemmatize
    
     Punctuations
    
     Remove numbers
    
     Remove stopwords
    


## 🧾 Results and solution

### Best model

TF-IDF Vectorizer with Logistic

Regression

    Max_df = 0.725
  
    Min_df = 0.0
  
    Ngram_range = (1,1)
  
    Smooth_idf = False
  
**Without train_test_split**

**Classifier:** Logisitic regression

**Parameters:** C = 2, ngram_range = (1,1), norm = 'l2'

**Accuracy:** 0.821


### Other models

**K-Nearest Neighbours (KNN) with TF-IDF**

Vectorizer

    K = 6
  
    Gridsearch not useful
  
    Score = 0.7559
  

**Decision Tree Classifier with TF-IDF**

    Default parameters

    Score = 0.6857

    No tuning hyper-parameters given low score
  
  
  **Random Forest with TF-IDF**

    Default parameters

    Score = 0.9466 

    No tuning hyper-parameters because this model is overfitted
  

## 📽️ Our video 
    
     [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/iFVyntNgX4A/0.jpg)](https://www.youtube.com/watch?v=iFVyntNgX4A)

# Data Science Analytics Virtual Intern at British Airways Co.
# _________________________________________________________

## First Task : Web scraping to gain company insights
### Scrape and analyse customer review data to uncover findings for British Airways

 ### - Scrape data from the web 
   #### i use a website called Skytrax. ( https://www.airlinequality.com/airline-reviews/british-airways )
   
 ### - Analyse data to uncover some insights
   #### After Reading the data, i perform some univarite analysis like see the distrubtion of Customer Rating 
   #### Create stopword list and visualize Wordcloud
   #### Classifying Reviews To 3 catigores ( Positive, Negative and Nutural )
   #### Data Cleaning by remove_punctuation
   #### create new Dataframe from the 2 important columns
   #### random split train and test data with numpy
   #### Create a bag of words with CountVectorizer from sklearn.feature_extraction.text
   
 ### - Modeling
   #### import RandomForestClassifier & Split target and independent variables
   #### Fit model on data and Make predictions
   #### find accuracy, precision, recall and make classification_report
 
 # _______________________________________________________________
 
 ## Second Task : Predicting customer buying behaviour
 ### Build a predictive model to understand factors that influence buying behaviour
 
 ### - Explore and prepare the dataset
 ####  First, spend some time exploring the dataset. then, Encode values labels for opject variables.
 
 ### - Modeling 
 #### * After preparing data, i do some feature engineering, then i Start with a Dummy Model (np.rand) - Baseline Model with accuarcy 0.49 and F1_score 0.22
#### * I try a Simple Model (linear) with :
#### Linear model & calculate score ( accuarcy 0.85 and F1_score 0.0 )
#### * Also i try a Simple Model with Balanced Dataset ( Upsampling[f1-score 0.24], Downsampling[f1-score 0.24] ).
#### * Then i try Complex and Explainable Modeles (Tree Based) :
 - #### Decision Tree (Original_data[f1-score 0.26], Upsampling[f1-score  0.30], Downsampling[f1-score 0.32] ).
 - #### Random Forest (Original_data[f1-score 0.13], Upsampling[f1-score  0.33], Downsampling[f1-score 0.38] ).
#### * Finally i try Deeper Modeles :
 - #### XGBoost (Original_data[f1-score 0.17], Upsampling[f1-score  0.34], Downsampling[f1-score 0.39] ).
 - #### CatBoost (Original_data[f1-score 0.11], Upsampling[f1-score  0.35], Downsampling[f1-score 0.40] ).

#### * The Best Model is : CatBoostClassifier With Downsampling data because the accuracy is higher.


# ______________________________________________________

 
 

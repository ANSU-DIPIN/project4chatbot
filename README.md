# project1reviews

# Project Name: Review Analysis for A product Listed on Amazon

# Contents

![image](https://user-images.githubusercontent.com/71720761/113471286-0cb3dd80-9479-11eb-856e-d8150a659451.png)


# 1.Introduction

* Reviews for a specific product are extracted . 

* Generated  insights from the text data by applying various text mining methods. 

* Sentiments (positive, negative, neutral, … are determined, by the model deployed, based on the new reviews from the website.  

# 2.Business Objective:

⮚	Natural Language processing on reviews of products in Amazon: Analyze the reviews posted by the customers and build an algorithm to find the emotions (Positive, Negative etc.,)

⮚	Classification of the reviews to be done on a weekly basis using the algorithm. Entire application should work Automatically.

# 3.DATA EXTRACTION

Extracted 5000 Amazon customer reviews of the product Boya-Omnidirectional-Lavalier-Condenser-Microphone
Saved the same as the csv file Review_MICROPHONE_new.csv.csv

![image](https://user-images.githubusercontent.com/71720761/113474730-58718180-948f-11eb-8501-70572642482b.png)

# 4.EDA

Bar Plots

![image](https://user-images.githubusercontent.com/71720761/113474846-f9f8d300-948f-11eb-8288-c481fee6d3ad.png)

![image](https://user-images.githubusercontent.com/71720761/113474857-0bda7600-9490-11eb-8fd1-d3fd2810d1e4.png)

Word Cloud for whole corpus

![image](https://user-images.githubusercontent.com/71720761/113474879-2b719e80-9490-11eb-9d6e-8f998321e65a.png)

Word Cloud for Positive and Negative words

![image](https://user-images.githubusercontent.com/71720761/113474908-55c35c00-9490-11eb-8b80-5b34adb88f4e.png)

![image](https://user-images.githubusercontent.com/71720761/113474912-5956e300-9490-11eb-95d2-9e4a0445901e.png)

# 5.MODEL BUILDING

We created the model using Stacking Classifier where base estimators (SVC,ExtraTreeClassifier,Logistic,LinearSVC) and final estimator(SVC) which resulted in the following for both balanced and unbalanced dataset.

# 6.Model Evaluation

When Data Is Imbalanced

![image](https://user-images.githubusercontent.com/71720761/113474980-b0f54e80-9490-11eb-8665-d008a94ccb90.png)

![image](https://user-images.githubusercontent.com/71720761/113474983-b6529900-9490-11eb-99c2-b65e42d834b9.png)

When Data Is Balanced

![image](https://user-images.githubusercontent.com/71720761/113474999-c9fdff80-9490-11eb-9d30-b5b5313c7ab4.png)

![image](https://user-images.githubusercontent.com/71720761/113475001-cd918680-9490-11eb-9e54-d83b0e084aeb.png)

# 7.Feedback

![image](https://user-images.githubusercontent.com/71720761/113475027-e437dd80-9490-11eb-9fd1-bc7f60ba2352.png)

![image](https://user-images.githubusercontent.com/71720761/113475030-e7cb6480-9490-11eb-99ce-214bbf683c18.png)

# 8.Deployment

Have used FLASK for deployment and have deployed Stack Classifier for deployment.

TFIDF and Model as been loaded in disk using pickle.

We will be using @app.route(‘/’) to execute home function which directly goes to home page which is created by html and is named by file home.html.

Then when predict is clicked it goes to @app.route(‘/predict’,methods=[POST]) to execute predict sentiment and given by file final.html.

The link for this whole deployment is given by http://127.0.0:5000.

![image](https://user-images.githubusercontent.com/71720761/113475064-12b5b880-9491-11eb-84fe-596a36be706b.png)

![image](https://user-images.githubusercontent.com/71720761/113475065-16493f80-9491-11eb-8eb9-2bf98ff6e417.png)


![image](https://user-images.githubusercontent.com/71720761/113475071-1fd2a780-9491-11eb-8776-66bbe2ca4be6.png)

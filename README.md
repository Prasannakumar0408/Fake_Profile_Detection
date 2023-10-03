**FAKE PROFILE DETECTION IN SOCIAL MEDIA PLATFORMS**

**INTRODUCTION**

Social media platforms have tens of millions of fake users, which puts users' security and privacy at risk. The Identification of fake users in these networks is crucial for improving user experience and safety. The interest in the verification of a legitimate profile is becoming more and more popular.

**OBJECTIVE**

The goal of this project is to create a model to recognize fake profiles on social media platforms based on the account type, followers, number of people following, date of registration, and other factors.

**DATA IDENTIFICATION**

This dataset taken from Kaggle contains information on 786 real users and false users of the Instagram social media network, together with 12 other parameters as follows, Profile Pic, Nums/Length Username, Fullname Words, Nums/Length Fullname, Name/Username, Description Length, External URL, Private, Posts, Followers, Follows, Fake.


**DATA VISUALIZATION**

The panda library, which is used for data analysis and manipulation, is first imported into the code. The train_test_split function from Sklearn's model_selection module is then imported, which is used to divide a dataset into training and testing sets. Each feature in this dataset only comprises 0s and 1s, and the dataset is free of null values. Before classifying anything, I made sure the target column was balanced. I'm using a bar plot to see if the dataset is balanced or not.

<img width="406" alt="image" src="https://github.com/Prasannakumar0408/Fake_Profile_Detection/assets/121532353/af9930d5-d915-4a1e-9feb-a301293a19e1">
<img width="393" alt="image" src="https://github.com/Prasannakumar0408/Fake_Profile_Detection/assets/121532353/7afbb1e7-212e-4807-9173-95129c5a294d">

The heatmap in the below plot illustrates the multicollinearity of the features, which is being checked to see which features should be dropped in order to improve the accuracy of false profile deduction.

<img width="462" alt="image" src="https://github.com/Prasannakumar0408/Fake_Profile_Detection/assets/121532353/fa1c4c6f-f0e0-4129-9abb-ac6e11e6d097">



**CLASSIFICATION MODELS**

We have used the following Machine-learning predictive models
1. Gaussian Naïve Bayes
2. KNN with Manhattan distance

**GAUSSIAN NAÏVE BAYES**


<img width="877" alt="image" src="https://github.com/Prasannakumar0408/Fake_Profile_Detection/assets/121532353/12561ca0-fec9-4a39-8c26-5de2853d9072">

**KNN WITH MANHATTAN DISTANCE**

<img width="868" alt="image" src="https://github.com/Prasannakumar0408/Fake_Profile_Detection/assets/121532353/65853ae0-cd80-4cae-bfa7-892c95c3a3ad">


**RESULT**


![image](https://github.com/Prasannakumar0408/Fake_Profile_Detection/assets/121532353/46e151c2-c7c4-45aa-bd31-4e8f156e25a4)

As demonstrated above, this prediction model is validated using two different classifiers. It can be seen clearly that KNN performs better than Gaussian model.



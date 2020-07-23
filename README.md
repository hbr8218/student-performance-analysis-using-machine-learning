# student-performance-analysis-using-machine-learning

## Table of Contents
* [Overview](#overview)
* [Motivation](#motivation)
* [Technical Aspect](#technical-aspect)
* [To Do](#to-do)
* [Bug Request](#bug-request)
* [Technoqies Used](#technologies-used)
* [Credits](#credits)
* [Citation Request](#citation-request)


## Overview
This is Analysis on student's performance and how the performance gets affected by differect factors. Analysis has been done in three datasets:- 
- My own college sample dataset.
- Two datasets from [UCI Machine learning repository](https://archive.ics.uci.edu/ml/index.php). </br>
This data approach student achievement in secondary education of two Portuguese schools. The data attributes include student grades, demographic, social and school related features) and it was collected by using school reports and questionnaires. Two datasets are provided regarding the performance in two distinct subjects: Mathematics (mat) and Portuguese language (por). In [Cortez and Silva, 2008], the two datasets were modeled under binary/five-level classification and regression tasks. Important note: the target attribute G3 has a strong correlation with attributes G2 and G1. This occurs because G3 is the final year grade (issued at the 3rd period), while G1 and G2 correspond to the 1st and 2nd period grades. It is more difficult to predict G3 without G2 and G1, but such prediction is much more useful (see paper source for more details).


## Motivation
Thinking about the final year project (B.TECH), A question came on my mind that why my college does not come in the categories of avarage colleges, why my college is not counted with India's top colleges > How the performance of students affect the college and what factors might be there which influenced the performance of the students. Thus, I decided to do a analysis on student's performance on sample dataset. Before that I had to do the same thing with a public dataset which I found in [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php) and got two datasets dealing with different factors affecting student's performace in two subjects i.e. Math and Portuguese Language.


## Technical Aspect
EDA(Extrapolatory Data Analysis) has been done on the datasets. Unlike my college's dataset, other two datasets have been studied in differents levels as follow:-
1. Binary Level classification:</br>
  In binary classification, students who got less than 10 are considered as fail and those who got more than or equal to 10 are considered as pass. Below graph may clear the picture </br>
 ![binary classification](https://user-images.githubusercontent.com/42790586/88254524-2f2f0d80-ccd3-11ea-9481-829661cdb2bd.png)
  
2.Five Level Classification: </br>
  if a student got x out of 20 where 0<=x<=20 <br>
then, <br>
x>=0 and x<=9 -> Fail <br>
x==10 or x==11 -> Sufficient <br>
x==12 or x==13 -> Satisfoctory <br>
x==14 or x==15 -> Good <br>
16<=x<=20 -> Excellent/Very Good <br>
![flcmath](https://user-images.githubusercontent.com/42790586/88255076-fdb74180-ccd4-11ea-886f-33551729644c.png)

3. Regression Modelling(Predictive G3/Final grade)
Different Machine learning algorithms like linear regression, ensemble techniques, catboots, xgboost,etc have been trained on two datasets(from UCI machine learning repository rather my college's dataset)  for predicting the Final grade i.e. G3 based on independent variables. 

## To Do
Following are the future planning with this project:-
1. A chatbot will be developed based on the model that can tell students to predict their performance and how their habbit may affect their performance and guide to pick up the important subjects for a given semester. (On going)
2. To deploy on cloud storage like AWS.

## Bug Request
If you have any suggestion, find any bug in the code  or have any query, feel free to contact me at hbr8218@gmail.com

## Technologies Used
- [Scikit-learn](https://scikit-learn.org/stable/index.html) has been used.
- Multiple pipline technique
- Data Normalization
- Principal Component Analysis(PCA)
- Clustering(K-Means) and Elbow-plot for finding reasonable number of clusters, etc.

## Credits
1. This project wouldn't have been possible without the assitance of my guru (Teacher/Guide/Tutor) Mr. Soumya Kanti Bhattacharya(Asst. prof, Computer Science Engineering branch, Bengal College of Engineering and Technology(West Bengal, India)) who help me through out project.
2. [UCI Machine Learning Repository]

## Citation Request
P. Cortez and A. Silva. Using Data Mining to Predict Secondary School Student Performance. In A. Brito and J. Teixeira Eds., Proceedings of 5th FUture BUsiness TEChnology Conference (FUBUTEC 2008) pp. 5-12, Porto, Portugal, April, 2008, EUROSIS, ISBN 978-9077381-39-7.
[<a href="http://www3.dsi.uminho.pt/pcortez/student.pdf">Web Link</a>]

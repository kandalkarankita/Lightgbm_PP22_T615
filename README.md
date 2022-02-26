# HDSC Winter ‘22 Premiere Project Presentation: Japan Trade Statistics 
## by Team LightGBM


![image](https://user-images.githubusercontent.com/76862496/155849808-44adc5b7-a229-4062-9c13-9888e1ea1c21.png)
Source: https://www.nippon.com/en/ncommon/contents/japan-data/133274/133274.jpg

### Table of Content
### 1.1	Introduction
### 1.2	About our Team
### 1.3	Problem Statement 
### 1.4	Aim of the Project
### 1.5	Methodology  
### 1.6	Exploratory Data Analysis
### 1.7	Building a Linear Model
### 1.8	Conclusion 



## 1.1 Introduction
Japan is a major trading nation as well as one of the world's largest international investors in terms of economic relations. International trade is the lifeblood of the Japanese economy in many ways. In 2017, Japan's imports and exports totaled nearly US$1.309.2 trillion, making it the world's fourth largest trading nation after China, the United States, and Germany. Trade was once the primary form of Japan's international economic relationships, but rapidly rising foreign investments added a new and increasingly important dimension in the 1980s, broadening the horizons of Japanese businesses and giving Japan new global prominence.

## 1.2 About our Team
This is an open-source project created for the Hamoye Data Science Internship. We are a group of data scientists, data storytellers, and data engineers, and each team member has a specific role to play.

## 1.3 Problem Statement
Japan is currently the 4th largest goods trading partner with $183.6 billion in total (two way) goods trade during 2020. Japan international trade and types of goods are captured in the months and years and stored in db files. As a data scientist required to help the management to make informed decisions by analyzing the data, and generate insights.

## 1.4 Aim of the Project
This project aims to analyze japan trade statistics got from Kaggle dataset and also to develop a linear regression model.

## 1.5 Methodology 
This section explains the steps or set of procedures that we followed during the project. Data collection, data description, data cleaning, EDA, and modeling are all part of this process.The dataset used in this project was gotten from Kaggle japan trade statistics. Notebook used in this project can be gotten from this Git repo.
COLUMN DEFINITION  
•	Exp_imp =export and import where exp=1 and imp=2  
•	hs2, hs4, hs6, hs9= products traded
•	Value= Revenue in $dollars
•	Q1= Quarter 1 sales
•	Q2= Quarter 2 sales


## 1.6 Exploratory Data Analysis
As with all real-world data, the dataset had some missing values and flaws, which necessitated data cleaning. Duplicate values were removed from the dataset. Below is visualization performed during EDA.

![image](https://user-images.githubusercontent.com/76862496/155849924-76436615-67e1-4a7b-9cbd-8a72c116000d.png)

### TOP 10 Trade markets in terms of values Year 2020


![image](https://user-images.githubusercontent.com/76862496/155849938-1ae1f5ad-efed-4afa-b5e3-648ece08f45a.png)

### Line plot of value over time (month) Year 2020


![image](https://user-images.githubusercontent.com/76862496/155849949-44375a41-fbfc-4614-ba25-996b4ce965e2.png)

### TOP 10 Trade markets over the year from 2017 to 2021


![image](https://user-images.githubusercontent.com/76862496/155849967-35e78f8e-e148-42a7-9c83-cb137201b520.png)

### TOP 10 Countries Japan exports the highest in terms of values Year 2017-2021


![image](https://user-images.githubusercontent.com/76862496/155849975-180fc08f-ee8c-48e9-a36d-1321f90fd2eb.png)

### TOP 10 Countries Japan imports the highest in terms of values Year 2017-2021


![image](https://user-images.githubusercontent.com/76862496/155849982-69fdd1e3-4715-4fcb-9668-bf6f89696ee3.png)

### Line plot of value over time (year)


### 1.7 Building a Linear Model

![image](https://user-images.githubusercontent.com/76862496/155849743-e89a7777-e1b8-4583-b43c-a17f0c6ff505.png)

### Heatmap of Correlation

As is visible from the pairplot and the heatmap, the variable Q2 seems to be most correlated with Values, so we performed simple linear regression using Q2 as our feature variable.
 
![image](https://user-images.githubusercontent.com/76862496/155849733-2ed1d00f-bf6e-41d4-a226-7ffbe82f6e75.png)

### Checking relationship between features and target variables


![image](https://user-images.githubusercontent.com/76862496/155849701-93fb0d7a-f16d-4281-9bba-79e2ce8fa59d.png)
 
### R2_score and MAE


### 1.9	Conclusion 
We have analysed Japan Trade Statistic and we found the top trade market over the years are; China,United_States_of_America,Korea,Taiwan,Australia,Thailand,Germany,Viet_Nam,Hong_Kong, Indonesia, and Malaysia. Most traded products are electronics, machines, vehicles, fuel, medical equipments, aircraft, aluminium, iron, chemicals among others. After training 70% of the data obtained a poor r2 score and poor correlation suggest the data is not good enough for predictions.

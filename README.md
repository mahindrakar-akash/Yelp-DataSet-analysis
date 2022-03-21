# Yelp-DataSet-analysis


Yelp dataset is used to research and analysis in investments on company, based on business and ratings how they impact. The dataset includes data about businesses, reviews. Here in my project I used review and business dataset.

Table of Contents
1. [Introduction](##introduction)
2. [Goal](##goal)
3. [Project Architecture](##project-architecture)
4. [ER Diagram](##er-diagram)
5. [Analysis](##analysis)

# 1. Introduction
This hadoop project is to apply some data engineering principles to Yelp Dataset in the areas of processing, storage, and retrieval.
In this Project, we will use the yelp review dataset to analyze businesses and reviews over a period of time. We will try to see which all business have highest rating and lowest rating.
Beyond processing this data, we will display the data in terms of graphs to let the leadership understand data in different dimensions.

# 2. GOAL
The main goal of this project is to provide an insight to the future investo/owner, on where and what business to invest in or where to start a new business based on the customer satisfaction.

# 3. Technology Stack
a. HDFS 
b. Hive 
c. Pyspark 
d. Flask

# 4. Bucket Calculation
Block Size in HDFS = 128 MB
Size of review dataset = 5120 MB
5120/128 = 40
2^x = 40 where x will be number of buckets
Hence we will take number of bucket = 6
Size of user dataset = 3205 MB
3205/128 = 25
2^x = 25 where x will be number of buckets
Hence we will take number of bucket = 5

# 5. Project Architecture



<img width="824" alt="Architechture" src="https://user-images.githubusercontent.com/100192179/159193250-2a1441d0-9a86-47b0-a073-a7bc6a580727.png">



# 6. ER Diagram

<img width="488" alt="image" src="https://user-images.githubusercontent.com/100192165/159173823-83af5ab2-fef5-45de-b0df-3dd04c551706.png">

# Analysis

 Top 10 Companies with good ratings
 
 
 
<img width="315" alt="image" src="https://user-images.githubusercontent.com/100192165/159175133-0bb36e91-ee31-4398-bda4-e50b8031889e.png">


Average stars rating of companies


<img width="319" alt="image" src="https://user-images.githubusercontent.com/100192165/159175286-c4b5e5a8-7ec7-401e-85fc-874a7f141e36.png">




Count of stars of each companies on which investment can be made.



<img width="319" alt="image" src="https://user-images.githubusercontent.com/100192165/159175347-193c75c8-e88f-4992-9761-90b5ec2c9868.png">

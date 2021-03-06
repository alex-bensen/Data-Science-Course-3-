# Data-Science-Course-3---
title: Run Analysis Codebook
author: Alex Bensen
date: 01/31/2022
---

This project takes training and test data from 30 different volunteers doing 6 different activities.  Data has been recorded on acceleration and velocity of the volunteers during their 6 activities. We recorded this data in the X, Y and Z directions. 
We first merged the training and test sets to create one data set.  Then we extracted the measurements on mean and standard deviation for each measurement.  We labeled each variable and activity accordingly and then made a final data set with the average of each variable for each activity and each subject.

The original, raw data was found in the train and test files, which contained data for each measurement collected on the volunteers as they were doing the different activities.  For the train and test data, we binded the y and subject files to the data frame as two different columns so we know the data recorded for each subject and activity.  Each row now indicates which subject and which activity the data was collected for.  

The final data set includes a column for each activity and each subject and a column for each variable being measured.  Each row correlates to a different variable (indicated by the 'Variables' column), and each column correlates to a different activity or subject.  So each cell gives a value for the average of a subject or activity and a variable that was measured.

Guide for create the data set:
1. read the X_test and X_train text files
2. merge the X_test and X_train text files
3. read the y_train, y_test, subject_train and subject_test files
4. merge the four text files into a dataframe with two columnes (subject and y columns)
5. rename the column names using the features.txt file
6. extract values for mean and std for each measurement using grepl function
7. rename the Activities column values from numbers to the actual name of activity
8. create subject and activity factors
9. use tapply() function to take mean of each variable based on subject and activity factors
10. create a dataframe that records the average of each variable for each activity and subject
11. add a column to indicate the variable for each row

General description of the dataframe:
 - 79 rows x 37 columns
 - dataframe provides averages of each variable for each acivity and subject
 - values:
        -Activities:
         Walking
         Walking_Upstairs 
         Walking_Downstairs 
         Sitting           
         Standing 
         Laying                 
         1: Subject 1
         2: Subject 2      
         3: Subject 3 
         4: Subject 4                
         5: Subject 5
         6: Subject 6                 
         7: Subject 7
         8: Subject 8                 
         9: Subject 9
         10: Subject 10               
         11: Subject 11
         12: Subject 12               
         13: Subject 13
         14: Subject 14               
         15: Subject 15
         16: Subject 16                
         17: Subject 17
         18: Subject 18               
         19: Subject 19
         20: Subject 20              
         21: Subject 21
         22: Subject 22                 
         23: Subject 23
         24: Subject 24     
         25: Subject 25
         26: Subject 26               
         27: Subject 27
         28: Subject 28              
         29: Subject 29
         30: Subject 30
             


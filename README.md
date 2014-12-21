coursera_getting_and_cleaning_data_project
==========================================

Introduction

This repository contains my work for the course project for the Coursera course "Getting and Cleaning data", part of the Data Science specialization. 

The  raw data that was used can be found in the following files:

The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

Here are the data for the project: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 


The features (561 of them) are unlabeled and can be found in the x_test.txt. The activity labels are in the y_test.txt file. The test subjects are in the subject_test.txt file.

The same holds for the training set.

This data was downloaded and placed in the following directory: ~classfiles/coursera_getting_and_cleaning_data_project
This script requires library(plyr)


A script called run_analysis.R was created which will do the following as required by the prroject: 

1)   Merges the training and the test sets to create one data set.
2)   Extracts only the measurements on the mean and standard deviation for each measurement. 
3)   Uses descriptive activity names to name the activities in the data set
4)   Appropriately labels the data set with descriptive variable names. 
5)   creates a second, independent tidy data set with the average of each variable for each activity and each subject.


The codebook explains what steps were taken to accomplish the items above.

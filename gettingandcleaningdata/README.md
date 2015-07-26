# README

## Course Project Introduction

Create R script called run_analysis.R that does the following

1. Merges the training and the test sets to create one data set
2. Extracts only the measurements on the mean and standard deviation for each measurement
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject

## Steps for the Course Project

1. Download the data source and put into a folder on the local drive
2. Put ```run_analysis.R``` in the parent folder of ```UCI HAR Dataset```, then set it as the working directory using ```setwd()``` function
3. Run ```source("run_analysis.R")```, then it will generate a new file ```tiny_data.txt``` in the working directory

## About the ```run_analysis.R```

* Require ```reshapre2``` and ```data.table``` librareis
* Load both the test and train data
* Load the features and activity labels
* Extract the mean and standard deviation column names
* Process the data
* Merge the data sets

## CodeBook

Describe the variables, the data, and any transformations or work that I performed to clean up the data

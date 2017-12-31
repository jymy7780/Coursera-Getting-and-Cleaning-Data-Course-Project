Getting and Cleaning Data - Course Project
==========================================

This repository hosts the R code and documentation files for the Coursera - Data Science Program, Course 3 "Getting and Cleaning data", Peer Graded Assignment.

The dataset being used is: [Human Activity Recognition Using Smartphones](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

Right click [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) and select "Save Link As" to download the the source data.

### Procedure

To prepare and clean the source data into the desired tidy data set,

1.  Download and Unzip the source file with the data into your R working directory.
  * Make sure that all the following files have unzipped into your R working directory.
    * features.txt
    * activity_labels.txt
    * X_train.txt
    * subject_train.txt
    * y_train.txt
    * X_test.txt
    * subject_test.txt
    * y_test.txt

2.  Copy "run_analysis.R" script into your R working directory.

3.  Install "dplyr" package in R.

4.  Run "run_analysis.R"

`CodeBook.md` describes the variables, the data, and any transformations or work that was performed to clean up the data.

### Information

`run_analysis.R` contains all the code to:
    
    1.  Merges the training and the test sets to create one data set.
    2.  Extracts only the measurements on the mean and standard deviation for each measurement.
    3.  Uses descriptive activity names to name the activities in the data set
    4.  Appropriately labels the data set with descriptive variable names.
    5.  From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

The tidy data output is `tidy_data.txt` in the UCI HAR Dataset folder.

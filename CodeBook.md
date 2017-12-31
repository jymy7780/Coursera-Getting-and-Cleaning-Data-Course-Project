Getting and Cleaning Data - Course Project CodeBook
===================================================

This CodeBook describes the structure and the variables of the output data set "tidy_data.txt", as a result of executing the "run_analysis.R" script.

For a comprehensive description of the dataset being used: [Human Activity Recognition Using Smartphones](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

Right click [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) and select "Save Link As" to download the the source data.

### Tidy data set description

30 Subjects were observed conducting 6 different activities.  Observation data was recorded to 66 diferent variables. Only Mean (mean():) and Standard Deviation (std():) values from the source data were retained.

The resulting data frame is composed of 180 observations (rows) and 68 variables (columns).  Each row has averaged variables for each subject and each activity.

### Tidy data set Variables.

1. Activity column has 6 types as listed below. Factor type.
    * WALKING
    * WALKING_UPSTAIRS
    * WALKING_DOWNSTAIRS
    * SITTING
    * STANDING
    * LAYING

2. "Subject"" column is numbered sequentially from 1 to 30. Integer type.

3.-68. Sensor Measurement Values. Numeric type.

3. "tBodyAcc-mean()-X"          
4. "tBodyAcc-mean()-Y"
5. "tBodyAcc-mean()-Z"
6. "tBodyAcc-std()-X"           
7. "tBodyAcc-std()-Y" 
8. "tBodyAcc-std()-Z"
9. "tGravityAcc-mean()-X"
10. "tGravityAcc-mean()-Y"
11. "tGravityAcc-mean()-Z"
12. "tGravityAcc-std()-X"        
13. "tGravityAcc-std()-Y"
14. "tGravityAcc-std()-Z"
15. "tBodyAccJerk-mean()-X"      
16. "tBodyAccJerk-mean()-Y"
17. "tBodyAccJerk-mean()-Z"
18. "tBodyAccJerk-std()-X"       
19. "tBodyAccJerk-std()-Y"
20. "tBodyAccJerk-std()-Z"
21. "tBodyGyro-mean()-X"         
22. "tBodyGyro-mean()-Y"
23. "tBodyGyro-mean()-Z"
24. "tBodyGyro-std()-X"          
25. "tBodyGyro-std()-Y" 
26. "tBodyGyro-std()-Z" 
27. "tBodyGyroJerk-mean()-X"     
28. "tBodyGyroJerk-mean()-Y"
29. "tBodyGyroJerk-mean()-Z"
30. "tBodyGyroJerk-std()-X"      
31. "tBodyGyroJerk-std()-Y"
32. "tBodyGyroJerk-std()-Z"
33. "tBodyAccMag-mean()"         
34. "tBodyAccMag-std()"
35. "tGravityAccMag-mean()"
36. "tGravityAccMag-std()"       
37. "tBodyAccJerkMag-mean()"
38. "tBodyAccJerkMag-std()"
39. "tBodyGyroMag-mean()"        
40. "tBodyGyroMag-std()"
41. "tBodyGyroJerkMag-mean()"
42. "tBodyGyroJerkMag-std()"     
43. "fBodyAcc-mean()-X"
44. "fBodyAcc-mean()-Y"
45. "fBodyAcc-mean()-Z"          
46. "fBodyAcc-std()-X"
47. "fBodyAcc-std()-Y"
48. "fBodyAcc-std()-Z"           
49. "fBodyAccJerk-mean()-X"
50. "fBodyAccJerk-mean()-Y"
51. "fBodyAccJerk-mean()-Z"      
52. "fBodyAccJerk-std()-X"
53. "fBodyAccJerk-std()-Y"
54. "fBodyAccJerk-std()-Z"       
55. "fBodyGyro-mean()-X"  
56. "fBodyGyro-mean()-Y"
57. "fBodyGyro-mean()-Z"         
58. "fBodyGyro-std()-X"
59. "fBodyGyro-std()-Y"   
60. "fBodyGyro-std()-Z"          
61. "fBodyAccMag-mean()"
62. "fBodyAccMag-std()"   
63. "fBodyBodyAccJerkMag-mean()" 
64. "fBodyBodyAccJerkMag-std()"
65. "fBodyBodyGyroMag-mean()" 
66. "fBodyBodyGyroMag-std()"     
67. "fBodyBodyGyroJerkMag-mean()" 
68. "fBodyBodyGyroJerkMag-std()"

### "run_analysis.R" variables

* x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
* x_total, y_total and subject_data merge the previous datasets to further analysis.
* selected_var, X_total extracts only the measurements on the mean and standard deviation for each measurement.
* colnames(Y_total), Y_total$activitylabel, activitylabel add descriptive activity names to the data set.
* colnames(X_total) appropriately labels the data set with descriptive variable names.
* colnames(Sub_total), total, total_mean creates a second, independent tidy data set with the average of each variable for each activity and each subject

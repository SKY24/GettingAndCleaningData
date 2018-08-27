# Getting and Cleaning Data Course Project

##### About this CodeBook
* This is for Coursera "Getting & Cleaning Data" Course Project
* Check README.md for general info.

##### Input Data
 * Global data
  * activity_labels.txt
  * features.txt
 * Data for each sample
  * [test|train]/X_[test|train].txt
  * [test|train]/y_[test|train].txt
  * [test|train]/subject_test.txt

##### Output Data
 * Clean data set named "tidydata.txt"
 * Data Fields for the clean data set
  * "activity"
    - activity been measured
  * "subject"
    - the ID of the test subject
  * "tBodyAcc-mean()-X"
  * "tBodyAcc-mean()-Y"
  * "tBodyAcc-mean()-Z"
  * "tBodyAcc-std()-X"
  * "tBodyAcc-std()-Y"
  * "tBodyAcc-std()-Z"
  * "tGravityAcc-mean()-X"
  * "tGravityAcc-mean()-Y"
  * "tGravityAcc-mean()-Z"
  * "tGravityAcc-std()-X"
  * "tGravityAcc-std()-Y"
  * "tGravityAcc-std()-Z"
  * "tBodyAccJerk-mean()-X"
  * "tBodyAccJerk-mean()-Y"
  * "tBodyAccJerk-mean()-Z"
  * "tBodyAccJerk-std()-X"
  * "tBodyAccJerk-std()-Y"
  * "tBodyAccJerk-std()-Z"
  * "tBodyGyro-mean()-X"
  * "tBodyGyro-mean()-Y"
  * "tBodyGyro-mean()-Z"
  * "tBodyGyro-std()-X"
  * "tBodyGyro-std()-Y"
  * "tBodyGyro-std()-Z"
  * "tBodyGyroJerk-mean()-X"
  * "tBodyGyroJerk-mean()-Y"
  * "tBodyGyroJerk-mean()-Z"
  * "tBodyGyroJerk-std()-X"
  * "tBodyGyroJerk-std()-Y"
  * "tBodyGyroJerk-std()-Z"
  * "tBodyAccMag-mean()"
  * "tBodyAccMag-std()"
  * "tGravityAccMag-mean()"
  * "tGravityAccMag-std()"
  * "tBodyAccJerkMag-mean()"
  * "tBodyAccJerkMag-std()"
  * "tBodyGyroMag-mean()"
  * "tBodyGyroMag-std()"
  * "tBodyGyroJerkMag-mean()"
  * "tBodyGyroJerkMag-std()"
  * "fBodyAcc-mean()-X"
  * "fBodyAcc-mean()-Y"
  * "fBodyAcc-mean()-Z"
  * "fBodyAcc-std()-X"
  * "fBodyAcc-std()-Y"
  * "fBodyAcc-std()-Z"
  * "fBodyAccJerk-mean()-X"
  * "fBodyAccJerk-mean()-Y"
  * "fBodyAccJerk-mean()-Z"
  * "fBodyAccJerk-std()-X"
  * "fBodyAccJerk-std()-Y"
  * "fBodyAccJerk-std()-Z"
  * "fBodyGyro-mean()-X"
  * "fBodyGyro-mean()-Y"
  * "fBodyGyro-mean()-Z"
  * "fBodyGyro-std()-X"
  * "fBodyGyro-std()-Y"
  * "fBodyGyro-std()-Z"
  * "fBodyAccMag-mean()"
  * "fBodyAccMag-std()"
  * "fBodyBodyAccJerkMag-mean()"
  * "fBodyBodyAccJerkMag-std()"
  * "fBodyBodyGyroMag-mean()"
  * "fBodyBodyGyroMag-std()"
  * "fBodyBodyGyroJerkMag-mean()"
  * "fBodyBodyGyroJerkMag-std()"

Description of steps undertaken to clean and reshape the data:

##### Step 0 Download, extract and read the data

##### Step 1 Read the files containing the labels for activities and features of vector

##### Step 2 Read the test & train data data
    * test/y_test.txt, test/subject_test.txt, test/X_test.txt
    * train/y_train.txt, train/subject_train.txt, train/X_train.txt
    
##### Step 3 Merge the training and the test sets

##### Step 4 Extract only the measurements on the mean and standard deviation for each measurement.
  * grep feature data frame to find the observations in interest, with their row ID. Those row IDs correspond to the column ID of "all_merged" data frame produced in Step 1
  * use select() to extract those targeted columns, in addition to the "activity" and "subject" columns

##### Step 5 Give descriptive activity names to name the activities in the data set
  
##### Step 6 Create a second, tidy data set with the average of each variable for each activity and each subject.

##### Step 7 : Final Step Write the new tidy data set

  * the new tidy data is written to "tidydata.txt"

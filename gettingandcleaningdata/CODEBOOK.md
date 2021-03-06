# CODEBOOK

## Source

* Original data: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
* Original description of the dataset: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## Information

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

## Data Sets

* 'README.txt'
* 'features.txt'
* 'features_info.txt'
* 'activity_labels.txt'
* 'test/X_test.txt'
* 'test/y_test.txt'
* 'test/subject_train.txt'
* 'test/Inertial Signals/total_acc_x_train.txt'
* 'test/Inertial Signals/total_acc_y_train.txt'
* 'test/Inertial Signals/total_acc_z_train.txt'
* 'test/Inertial Signals/body_acc_x_train.txt'
* 'test/Inertial Signals/body_acc_y_train.txt'
* 'test/Inertial Signals/body_acc_z_train.txt'
* 'test/Inertial Signals/body_gyro_x_train.txt'
* 'test/Inertial Signals/body_gyro_y_train.txt'
* 'test/Inertial Signals/body_gyro_z_train.txt'
* 'train/X_train.txt'
* 'train/y_train.txt'
* 'train/subject_train.txt'
* 'train/Inertial Signals/total_acc_x_train.txt'
* 'train/Inertial Signals/total_acc_y_train.txt'
* 'train/Inertial Signals/total_acc_z_train.txt'
* 'train/Inertial Signals/body_acc_x_train.txt'
* 'train/Inertial Signals/body_acc_y_train.txt'
* 'train/Inertial Signals/body_acc_z_train.txt'
* 'train/Inertial Signals/body_gyro_x_train.txt'
* 'train/Inertial Signals/body_gyro_y_train.txt'
* 'train/Inertial Signals/body_gyro_z_train.txt'

## Features Selection

These signals were used to estimate variables of the feature vector for each pattern 
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions

* tBodyAcc-XYZ
* tGravityAcc-XYZ
* tBodyAccJerk-XYZ
* tBodyGyro-XYZ
* tBodyGyroJerk-XYZ
* tBodyAccMag
* tGravityAccMag
* tBodyAccJerkMag
* tBodyGyroMag
* tBodyGyroJerkMag
* fBodyAcc-XYZ
* fBodyAccJerk-XYZ
* fBodyGyro-XYZ
* fBodyAccMag
* fBodyAccJerkMag
* fBodyGyroMag
* fBodyGyroJerkMag

The set of variables that were estimated from these signals are

* mean(): Mean value
* std(): Standard deviation
* mad(): Median absolute deviation 
* max(): Largest value in array
* min(): Smallest value in array
* sma(): Signal magnitude area
* energy(): Energy measure. Sum of the squares divided by the number of values 
* iqr(): Interquartile range 
* entropy(): Signal entropy
* arCoeff(): Autorregresion coefficients with Burg order equal to 4
* correlation(): correlation coefficient between two signals
* maxInds(): index of the frequency component with largest magnitude
* meanFreq(): Weighted average of the frequency components to obtain a mean frequency
* skewness(): skewness of the frequency domain signal 
* kurtosis(): kurtosis of the frequency domain signal 
* bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window
* angle(): Angle between to vectors

Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable

* gravityMean
* tBodyAccMean
* tBodyAccJerkMean
* tBodyGyroMean
* tBodyGyroJerkMean

The complete list of variables of each feature vector is available in 'features.txt'

## Activity Lables

* WALKING
* WALKING_UPSTAIRS
* WALKING_DOWNSTAIRS
* SITTING
* STANDING
* LAYING

## Transformation details

1. Merges the training and the test sets to create one data set
2. Extracts only the measurements on the mean and standard deviation for each measurement
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject



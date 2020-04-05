# GettingAndCleaningDataProj Read Me
## Data description
The variables in the data X are sensor signals measured with waist-mounted smartphone from 30 subjects.
The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. Training and test data were first merged together to create one data set, then the measurements on the mean and standard deviation were extracted for each measurement (79 variables extracted from the original 561), and then the measurements were averaged for each subject and activity, resulting in the final data set.
The variable in the data Y indicates activity type the subjects performed during recording.

## Code explaination

The code combined training dataset and test dataset, and extracted partial variables to create another dataset with the averages and std dev of each variable for each activity.

## New dataset

The new generated dataset contained variables calculated based on the mean and standard deviation. Each row of the dataset is an average of each activity type for all subjects.

The code was written based on the instruction of this assignment

The R script called run_analysis.R does the following.
<ol>
<li>Merges the training and the test sets into one data set.
<li>Extracts only the measurements on the mean and standard deviation for each measurement.
<li>Uses descriptive activity names to name the activities in the data set
<li>Appropriately labels the data set with descriptive variable names.
<li>From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
</ol>
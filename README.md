# Course-Project-Week-4

The data used in this lesson correspond to a Human Activity Recognition database built from the recordings of 30 subjects performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors.
For more information visit: 
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

**Run_analysis.r**

The included script has the purpose of obtaining and cleaning data, performing the following steps in general: (It should be mentioned that the main library used is dplyr)

Before performing these steps, code is included to download the zip and unzip it.
It is important to mention that in the data extraction, the "Inertial Signals" folder is excluded as it is considered unnecessary, since then the data is selected by mean and std.

1.-Merges the training and the test sets to create one data set.

2.-Extracts only the measurements on the mean and standard deviation for each measurement.

3.-Uses descriptive activity names to name the activities in the data set

4.-Appropriately labels the data set with descriptive variable names.

5.-From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.



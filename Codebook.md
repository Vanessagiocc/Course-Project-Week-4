# <u>Codebook</u>

This CodeBook describes the variables, the data, and any transformations or work performed to clean up the data.

## The data

- Subjects: Group of 30 volunteers. 1 to 30.
- Activitys: Six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING)
- Features: The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. There are a total of 561 features.

## The variables

activity_label: Include the class labels with their activity name.

features: Include all the features

subject_test/train: Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30. 

x_test/train: The measurements

y_test/train: Activity labels.



Type: Character vector, indicates the type of measurement, "Train" or "Test".

Datatest: Data.frame, includes the subject, activity label, measurement and type of the test data.

Datatrain: Data.frame, includes the subject, activity label, measurement and type of the train data.

Data_total: Data.frame, includes the subject, activity label (Replaced by activity name later), type and measurement of the mean and std features.

tidy_data: Data.frame, includes the average of each variable for each activity and each subject.

## Transformations

Data_total is created and then a chaining code is used that selects some columns and specifically matches the ones that contain the words "mean" or "std".

Then the Activity column is updated, where the activity label or number is replaced with the name of the activity from the activity_labels data frame, using sapply.

Finally, a new data.frame, called tidy_data, is created from Data_total, using chaining, and the functions group by, and summary_at, excluding the Type column and calculating the average or mean.
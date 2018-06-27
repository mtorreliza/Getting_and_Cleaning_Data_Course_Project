=====================

This codebook explains all tables, datasets, vriable names used in this project

#Tables Definition

subject_test - contains subjects of the test experiment

X_test - contains all the observations for test

y_test - contains the activity data for test

subject_train - contains subjects of the train experiment

X_train - contains all the observations for train

y_train - contains the activity data for train

activity_labels - contains activity descriptive names

features - contains all variable names for all observations

#Datasets

measurement - merged test and train data observations (X_test,y_test)

activity - merged test and train activity data (y_test,y_train)

subject - merged test and train subject data (subject_test,subject_train)

MeanStd - list of variable names containing mean() and std() measures

dataset - merged measurement, activity and subject data

dataset_final - contains the tidy data formed from melting and casting

The final dataset contains 4 variables: subject, activity, measure, average

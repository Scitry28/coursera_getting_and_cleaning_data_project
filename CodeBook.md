Introduction


The script run_analysis.R performs the 5 steps described in the course project's definition as outlined in the README.md.

First, all the similar data is merged using the rbind() function. By similar, we address those files having the same number of columns and referring to the same entities.

All the data is read in and then similar data (same number of columns and referring to the same entities) is merged using the rbind() function.  This is for both training and test data files until we have one merged file.

Columns with the mean and standard deviation measures only are taken from the dataset of all the merged data. This is done by parsing the dataset with the grep() function.  Then the correct names from features.txt are applied to the columns we extracted. Using names() and the features data fram created earlier.



We then substitue activity names and IDs from activity.labels.txt in  a similar fashion and clean up any other column names.

Lastly a new dataset is generated with avearge measures for each subject and activity.



Variables
1.    x_train, y_train, x_test, y_test, subject_train and subject_test contain the data which was downloaded

2.    x_data, y_data and subject_data represent the merged datasets as requested in step 1. 

3.    The "features" df " contains the correct names for the x_data dataset, these are then applied to column names mean_and_std_features (a numeric a numeric vector     used for selection)  activity names are applied in te same fashion.

4.    All three data frames (x_data, y_data and subject_data) are merged by column using cbind()

5.     Average_data is a data frame that has all the relevant averages,  ddply() of Plyr() has a col_means function which simplifies the operation of creating this data frame

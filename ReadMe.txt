This R script is part of the Coursera Data Science Specialization Final Project. The project involves working with data from the UCI Human Activity Recognition Using Smartphones Dataset. The script downloads and processes the dataset, creating a tidy dataset that summarizes mean values for selected variables related to accelerometer and gyroscope measurements.

Download and Extract Data

The script checks if the project archive file (Coursera_DS3_Final.zip) and the extracted folder (UCI HAR Dataset) already exist to avoid redundant downloads and extractions. If not, it downloads the archive file from a specified URL and extracts its contents into the working directory.

Read Data

The script reads various files from the dataset, including features, activity labels, and training/test data for subjects, X (feature variables), and Y (activity labels).

Merge and Tidy Data

The script combines the training and test datasets, extracts only the mean and standard deviation variables, and performs some renaming operations to improve variable names.

Generate Final Tidy Data

Finally, the script creates a new dataset (FinalData) by grouping the tidy data by subject and activity and calculating the mean for all variables. The resulting dataset is written to a file (FinalData.txt) without row names.

Variable Descriptions

features: Contains the names of the features measured in the dataset.
activities: Maps activity codes to their corresponding labels.
subject_test: Contains subject IDs for the test dataset.
x_test: Contains feature variables for the test dataset.
y_test: Contains activity labels for the test dataset.
subject_train: Contains subject IDs for the training dataset.
x_train: Contains feature variables for the training dataset.
y_train: Contains activity labels for the training dataset.
X: Merged feature variables from the training and test datasets.
Y: Merged activity labels from the training and test datasets.
Subject: Merged subject IDs from the training and test datasets.
Merged_Data: Combined dataset with subject IDs, activity labels, and feature variables.
TidyData: Subset of the merged data, including only mean and standard deviation variables.
FinalData: Final tidy dataset, aggregating mean values by subject and activity.
# Getting And Cleaning Data - Peer Accessment CookBook
Getting-and-Cleaning-Data Peer Assessment CookBook file.

This file describe the data, variable and wprk that I performed on the data.

<ul>
  <li>Data is downloaded from the link: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and unzip in the working directory</li>
  <li>R script begins with having trainData, trainLabel, trainSubject which stored data from X_train.txt, y_train.txt and subject_train.txt</li>
  <li>Next is having testData, testLabel, testSubject which stored data from X_test.txt, y_test.txt and subject_test.txt </li>
  <li>Use rbind to join data and get data frame; joinData, joinLabel and joinSubject</li>
  
  <li>Read features.txt and stored data in features.</li>
  <li>Extract based on the measurements on the mean and standard deviation. I have a subset, joinData. Rename the subset.</li>
  
  <li>Read activity_labels.txt and stored data in activity.</li>
  <li>Use descriptive activity names to name the activities in the data set. </li>
  
  <li>Transform the values of joinLabel according to the activity data frame. Join joinData, joinLabel and joinSubject to have a data set.</li>
  <li>Then, data frame named as cleanedData. Use write.table to write the cleanedData out to "merged_data.txt" file in my current working directory. </li>
  
  <li>Create a second, independent tidy data set with the average of each variable for each activity and each subject.</li>
  <li>There are 6 activities in total and 30 subjects in total, we have 180 rows of records. Work around with data frame named result.</li>
  <li>Use write.table to write out to "data_with_means.txt" file in my current working directory. </li>
</ul>

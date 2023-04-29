
    Download the dataset
        Dataset downloaded to UCI HAR Dataset in ~/

    Assign data
        features <- features.txt 
        activities <- activity_labels.txt
        subject_test <- test/subject_test.txt 
        x_test <- test/X_test.txt 
        y_test <- test/y_test.txt
        subject_train <- test/subject_train.txt
        x_train <- test/X_train.txt
        y_train <- test/y_train.txt

    rBind() merges data sets
    
    Takes the mean and standard deviation for each measurement
        TidyData is created by subsetting Merged_Data, selecting only columns: subject, code and the measurements on the mean and standard deviation (std) for each measurement

    Assigns descriptive activity names to name the activities in the data set
      
    Creates a tidy data set with the average of each variable for each activity and each subject
      
        FinalData is created by sumarizing TidyData taking the means of each variable for each activity and each subject, after grouped by subject and activity.
        
    Exports FinalData into FinalData.txt file.

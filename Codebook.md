Data Dictionary for "combinedData.txt"

activity
     WHAT SUBJECT WAS DOING WHEN MEASUREMENT WAS TAKEN
     
        WALKING
        WALKING_UPSTAIRS
        WALKING_DOWNSTAIRS
        SITTING
        STANDING
        LAYING
        
subject
     UNIQUE IDENTIFIER FOR EACH PARTICIPANT IN STUDY
        1...30
        
79 variables of the form t...meanX, f...meanX, t...stdX (for list of full variable/column names see below)
        
"tBodyAccmeanX"               
"tBodyAccmeanY"                "tBodyAccmeanZ"                "tGravityAccmeanX"            
"tGravityAccmeanY"             "tGravityAccmeanZ"             "tBodyAccJerkmeanX"           
"tBodyAccJerkmeanY"            "tBodyAccJerkmeanZ"            "tBodyGyromeanX"              
"tBodyGyromeanY"               "tBodyGyromeanZ"               "tBodyGyroJerkmeanX"          
"tBodyGyroJerkmeanY"           "tBodyGyroJerkmeanZ"           "tBodyAccMagmean"             
"tGravityAccMagmean"           "tBodyAccJerkMagmean"          "tBodyGyroMagmean"            
"tBodyGyroJerkMagmean"         "fBodyAccmeanX"                "fBodyAccmeanY"               
"fBodyAccmeanZ"                "fBodyAccmeanFreqX"            "fBodyAccmeanFreqY"           
"fBodyAccmeanFreqZ"            "fBodyAccJerkmeanX"            "fBodyAccJerkmeanY"           
"fBodyAccJerkmeanZ"            "fBodyAccJerkmeanFreqX"        "fBodyAccJerkmeanFreqY"       
"fBodyAccJerkmeanFreqZ"        "fBodyGyromeanX"               "fBodyGyromeanY"              
"fBodyGyromeanZ"               "fBodyGyromeanFreqX"           "fBodyGyromeanFreqY"          
"fBodyGyromeanFreqZ"           "fBodyAccMagmean"              "fBodyAccMagmeanFreq"         
"fBodyBodyAccJerkMagmean"      "fBodyBodyAccJerkMagmeanFreq"  "fBodyBodyGyroMagmean"        
"fBodyBodyGyroMagmeanFreq"     "fBodyBodyGyroJerkMagmean"     "fBodyBodyGyroJerkMagmeanFreq"
"tBodyAccstdX"                 "tBodyAccstdY"                 "tBodyAccstdZ"                
"tGravityAccstdX"              "tGravityAccstdY"              "tGravityAccstdZ"             
"tBodyAccJerkstdX"             "tBodyAccJerkstdY"             "tBodyAccJerkstdZ"            
"tBodyGyrostdX"                "tBodyGyrostdY"                "tBodyGyrostdZ"               
"tBodyGyroJerkstdX"            "tBodyGyroJerkstdY"            "tBodyGyroJerkstdZ"           
"tBodyAccMagstd"               "tGravityAccMagstd"            "tBodyAccJerkMagstd"          
"tBodyGyroMagstd"              "tBodyGyroJerkMagstd"          "fBodyAccstdX"                
"fBodyAccstdY"                 "fBodyAccstdZ"                 "fBodyAccJerkstdX"            
"fBodyAccJerkstdY"             "fBodyAccJerkstdZ"             "fBodyGyrostdX"               
"fBodyGyrostdY"                "fBodyGyrostdZ"                "fBodyAccMagstd"              
"fBodyBodyAccJerkMagstd"       "fBodyBodyGyroMagstd"          "fBodyBodyGyroJerkMagstd"     

        The values these variables take in the tidy data set are the means of the observations for each                                 
        activity for each subject. The values range between -1 and 1. There are no units because as stated         
        in one of the forum discussions, "with all the variables, the data has been divided by its range 
        (gyroscope, entropy, etc) to normalise it. When you divide something with a set of units by 
        something else using the same set of units, the units are cancelled out leaving you with a ratio"
        
        The original, more complete description of the data used to compute the means of these variables is                 
        available in "features_info.txt". Please consult that file for a fuller understanding of how the         
        data was generated.
The script run_analysis.R assumes that the following files from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip have been loaded into the working directory:

"subject_test.txt"
"X_test.txt"
"y_test.txt"
"features.txt"
"activity_labels.txt"
"subject_train.txt"
"X_train.txt"
"y_train.txt"

When the script is run in R:

The script assigns the column names from "features.txt" to the files. I did this at the beginning because it helped me to see what was going on more easily than leaving them as "V1" "V2", etc.

Then all the data for the "test" files is bound together, followed by the "train" data, creating two data frames of 563 variables and differing numbers of observations. These two data frames are then bound together to create one data frame called "combined" with 10,299 observations on 563 variables.

Next the script assigns descriptive activity names from the "activity_labels.txt" file to name the activities in the data set. 

To appropriately label the data set with descriptive variable names, the characters "(", ")", and "-" are removed. Otherwise the column labels are left the same because to make them more descriptive by expanding the abbreviations would make them too long and make the dataset look cluttered.

I dealt with all this naming and name cleanup here because, again, it helped me to more clearly see what was going on as I developed the script and checked the results. Most likely it could have been done elsewhere without any negative effects.

Once all the combining and labeling is finished, the script uses the reshape2 package to melt the data and extract the columns dealing with the means and standard deviations. 

Then it casts the data into a tidy data set with 180 observations on 81 variables, called "combinedData". That data set is output as a text file called "combinedData.txt" using write.table(), which can be read back into R using read.table().


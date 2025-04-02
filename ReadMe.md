Using DataFrames and Spark SQL			 12 Points

Problem 3. 
Consider the DataFrame.scala or DataFrame.ipynb scripts together with the titanic.csv
dataset provided on Moodle to solve this problem.

(a) Create a user-defined function (UDF) called MedianAge that computes the median age over all
passengers in the initial Spark DataFrame. Your function should automatically replace all null
entries for the passengers’ ages with the default integer value “23” while calculating the median age.
Refer to the “User-Defined Aggregate Functions (UDAFs)” section in the Spark SQL programming
guidelines2 for an example.			 4 Points

(b) Implement the following query using only built-in DataFrame and/or SQL operations. Refer to the
Spark SQL documentation3 for the list of operations that can be performed on a DataFrame.
Query: “Select the name and fare price of all passengers whose age is greater than the median age
of all passengers who embarked on the Titanic.”  4 Points

(c) Assume we wish to investigate the following (statistical) hypothesis:
Hypothesis: “The average fare price of passengers who survived the sinking of the Titanic is not
very different from (i.e., neither much below nor much above) the average fare price of passengers
who did not survive the sinking of the Titanic.”
How would you verify the above hypothesis? Please provide an implementation based on Spark’s
built-in DataFrame and/or SQL operations. You may but you do not have to use a statistical test
(such as the “Unequal Variance T-Test”) to either accept or reject this hypothesis; a simple numeric
comparison will also be sufficient. Summarize your results in your Problem 3.txt file. 					4 Points

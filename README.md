# Getting and Cleaning Data Course Project

About this README
--------

* This is for Coursera  "Getting & Cleaning Data" Course Project
* The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis.
* This README describes the technical assumptions to run the R script
* Running the R script is specified
* The way to check the output result is also specified

- UCI HAR Dataset -> 		folder which contains the raw data to be processed.
						The link of the data:
						http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
            
            You can download as:
            https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
            
	- tidydata.txt ->	text file which contains the tidy data set after cleaning.
	- CodeBook.md ->	markdown	file that describes the variables, and data
	- run_analysis.R ->	script to process data.

Codebook
--------

To see more information on the analysis implemented, please see the MarkDown file `CodeBook.md`.

Run the R script
--------

You need "dplyr" package and internet 


You can open R console and load the script file
~~~
$ R
...
> source('run_analysis.R')
~~~

or you can open R Studio and load the script from there
either from command line
~~~
> source('run_analysis.R')
~~~
or from the menu "File" -> "Open File" and choose "run_analysis.R"
Ctrl-A to choose all, and Ctrl-Enter to run the selected script

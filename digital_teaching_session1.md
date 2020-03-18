# Digitial Teaching sessions March 2020


## Getting data with cURL

**In this lesson we use the cURL command in Git to get data down from an online repository and save
a copy on our computer**


**Objectives**

Using cURL in Git

Introduciton to Datahub.io

Refreshing how to make a directory, save and rename a file in Git



**What is cURL**

cURL transfers data from one server to another, is used to test APIs and download files

In Git, write curl --help to see all the options there are with cURL.



**Finding data**

Go to Datahub.io. This is a collection of open datasets, primarily in csv and json formats. Scroll

down the home page to browse the categories of datasets or use FIND DATA to find a specific set.

Datahub.io constructs URLs using publisher and dataset name, and has guides to using R, Python 

and cURL.

In this exercise we are using the data set https://datahub.io/core/registry

The registry dataset is a overview of all the open data sets on Datahub.io.

Go to the landing page for the registry data set. Scroll down to core-list and copy the

Share url to the clipboard. https://datahub.io/core/registry/r/0.html



**Back in Git**

Make sure you are in the directory you want to store the downloaded data in.

Make a new folder mkdir curl

Activate that folder cd curl

Remember: to navigate the file structure use the commands pwd, cd, /c/, /p/



**Previewing the data**

Before we download the data, let's have a look at it.

curl --head  gives you information about the content, type, length and provenence of the data

The script looks like this curl --head https://datahub.io/core/registry/r/0.csv

Note that I have changed the file type from html to csv. You could also write the following

to get the heading from the json file: https://datahub.io/core/registry/r/0.json



**Downloading the data**

We download using the -L flag. This flag means location. It recolate and redirects our request until we

get to the data. the script is:

curl -L https://datahub.io/core/registry/r/0.csv

OR

https://datahub.io/core/registry/r/0.json

OR if we want to get the metadata AND the data https://datahub.io/core/registry/datapackage.json



**Saving the file locally**

To save a copy of the data locally use the -O flag. 

curl -LO https://datahub.io/core/registry/r/0.csv

To see the files use the ls command. You should have a file called 0.csv. This is not very informative.

Let's change the name:

mv 0.csv Registry.csv



## Well done!! 

You have located data in an online repository, downloaded and saved a copy locally, in a file 
structure where you can find it again.














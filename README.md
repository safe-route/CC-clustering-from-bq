# Clustering Job from Big Query
A python code for clustering data from source (big query table of crime data) and the write it to JSON.

## Overview
This code is for implementation step 1 of project that make a JSON file for clustering from Big Query and save it to Cloud Storage. This code will be implemented in Cloud Function.

##Running the Program
###In Cloud Function
In cloud function, just download or copy the code to code section and requirement to requirement section and adjust the big query table to the table that has been provided. Before that because there is no direct trigger to big query, you need to set the big query succeed logging to pubsub and set the trigger type in cloud function as cloud pub/sub and set other settings as needed, then set the entry point to main and deploy the function.

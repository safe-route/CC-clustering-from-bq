# Clustering Job from Big Query
This is a python code for clustering data from source (big query table of crime data) and the write it to JSON.

## Summary
A function to create a JSON file that contain the list of crime that happen in a centroid. This is using big query as a source data and then the data from big query processed by the centroid model to create a JSON file and save it to Cloud Storange.

## Reference
By following Google's recommendation of building cloud functions development environment [here](https://cloud.google.com/functions/docs/running/overview), and by following the code examples [here](https://cloud.google.com/functions/docs/calling/http#functions-calling-http-nodejs), to act as a basis for the code development environment.

The development environment of this function is initiated by using project wide python's [virtual environment](https://docs.python.org/3/library/venv.html#:~:text=A%20virtual%20environment%20is%20a,part%20of%20your%20operating%20system.), and usage of [pip](https://pypi.org/project/pip/).

This function will run in cloud function and following the code examples [Cloud Function Trigger by Big Query](https://stackoverflow.com/questions/54792976/trigger-cloud-function-when-new-data-in-bigquery)

## Running the Program

### In Cloud Function
In cloud function, just download or copy the code to code section and requirement to requirement section and adjust the big query table to the table that has been provided. Before that because there is no direct trigger to big query, you need to set the big query succeed logging to pubsub and set the trigger type in cloud function as cloud pub/sub and set other settings as needed, then set the entry point to main and deploy the function.



# Operatinalizing Machine Learning using Azure

*TODO:* The main objective of the this project to deploy machine learning at work. In the project we are training the machine learning model AutoML by Azure. The benefit of AutoML is that it will select the best model from the a lot of machine learning algorithm. It will give best trained model. After getting best best model we will deploy the best model using Azure Kubernate service. We will also consume the model using Swagger

## Architectural Diagram
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/Azure%20ML%20Project%202.jpg)
## Key Steps
## Step 1: Automated ML Experiment
In the first step we are getting the data to Azure Machine Learning. After the data is uploaded, it will be available in dataset
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/1.JPG)

We are giving the job of determing the best model to Azure Auto ML. Azure Auto ML will run a nuber of available machine learning model and select the best machine learning model based on primary metric. We have selected accuracy as primary metric
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/2.JPG)

Once the run of Auto ML is completed we can check the final model and accuracy of the model. We can check in experiment if Auto ML is completed 
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/3.JPG)

## Step 2: Deploy the best model
The best model is selected from Azure Auto ML run. After selecting the best, the model is deployed. From this experiment Voting Ensemble is the best model with accuracy of 91.6%. 
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/4.JPG)

After selecting the best model, we are deploying the model using Azure Container Instance. 
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/5.JPG)
## Step 3: Enable App Insights & Logging
Sometimes the deployed may get some issue in production hence we are enabling application insights logs by enabling application insights
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/6.JPG)
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/7.JPG)
## Step 4: Swagger Documentation 
As our machine learning model is taking input in json, swagger documentation can help us to understand the input and output of deployed machine model. The latest version of swagger was downloaded using swagger.sh and python server was run on local server. We have used swagger.json file proived my Azure after deploying the machine learning model

![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/8.JPG)
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/9.JPG)
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/10.JPG)
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/11.JPG)
## Step 5: Consumption
Although there are multiple way to consume deployed model.Here we are using python to consume the machine learning model. We are sending some data points and getting the predictions from the deployed model
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/12.JPG)
## Step 5: Pipeline 
Pipeline is very important for automation of machine learning task. We are creating pipeling for training of our model using jupyter notebook
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/13.JPG)
After completion of pipeline run it is also deployed and it can be consumed using enpoints 
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/14.JPG)
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/15.JPG)
![alt text](https://github.com/agshiv92/Azure_ML_project-2/blob/main/16.JPG)
## Screen Recording
[![IMAGE ALT TEXT](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://studio.youtube.com/video/_9oU2V9Hs98 "Video Title")
Please click here for screen recording

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.

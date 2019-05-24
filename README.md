
## Project Overview

It is the Deploying A Sentiment Analysis Model Using SageMaker project from the Deep Learning Nanodegree program of Udacity. This project is based on a RNN model that classifies films reviews in positive or negative ones. This model is deployed by using SageMaker and it has an interface with a web page where the user can enter a review. The web page will then send the review off to our deployed model which will predict the sentiment of the entered review and sill send back to the web page the prediction. The daset used in this proyect is the lMDb dataset.

## Project Instructions

The notebook of the current proyect is intendeed to be executed in the Amazon SageMaker platform. The following is a brief set of instructions on setting up a managed notebook instance using SageMaker.

### Log in to the AWS console and create a notebook instance

Log in to the AWS console and go to the SageMaker dashboard. Click on 'Create notebook instance'. The notebook name can be anything and using ml.t2.medium is a good idea as it is covered under the free tier. For the role, creating a new role works fine. Using the default options is also okay. Important to note that you need the notebook instance to have access to S3 resources, which it does by default. In particular, any S3 bucket or objectt with sagemaker in the name is available to the notebook.

### Use git to clone the repository into the notebook instance
Once the instance has been started and is accessible, click on 'open' to get the Jupyter notebook main page. We will begin by cloning the SageMaker Deployment github repository into the notebook instance. Note that we want to make sure to clone this into the appropriate directory so that the data will be preserved between sessions.

Click on the 'new' dropdown menu and select 'terminal'. By default, the working directory of the terminal instance is the home directory, however, the Jupyter notebook hub's root directory is under 'SageMaker'. Enter the appropriate directory and clone the repository as follows.

	cd SageMaker

	git clone https://github.com/HebertoMadrigalSastre/DLNP_P5_Deploying_A_Sentiment_Analysis_Model.git

	exit


After you have finished, close the terminal window.

### Open and run the notebook
Now that the repository has been cloned into the notebook instance. Now, you can open the 'SageMaker Project.ipynb' notebook and execute it.


*For more details, please refer to the README.md file of the [udacity/sagemaker-deployment](https://github.com/udacity/sagemaker-deployment)* repository.


## Project content

Content: 

- Step 1: Downloading the data
- Step 2: Preparing and Processing the data
- Step 3: Upload the data to S3
- Step 4: Build and Train the PyTorch Model
- Step 5: Testing the Model
- Step 6: Deploying the model for testing
- Step 7: Use the model for testing
- Step 6 (again): Deploy the model for the web app
- Step 7 (again): Use the model for the web app

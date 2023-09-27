# - Serverless image processing application
This serverless application can be used to resize and compress images. It is triggered by new images being uploaded to a cloud storage bucket and uses AWS services such as S3, Lambda, and Step Functions to orchestrate the image processing workflow.

The application works as follows:

A new image is uploaded to the S3 bucket.
The S3 event triggers the Step Functions state machine.
The Step Functions state machine invokes the Lambda function to resize and compress the image.
The Lambda function resizes and compresses the image and uploads the processed image to S3.
The Step Functions state machine completes successfully.
The application is written in Python 3.8 and uses the following AWS services:

S3: To store the original and processed images.
Lambda: To resize and compress the images.
Step Functions: To orchestrate the image processing workflow.
To use the application, you will need to:

Create an S3 bucket to store the original and processed images.
Create a Lambda function to resize and compress the images.
Create a Step Functions state machine to orchestrate the image processing workflow.
Configure the Step Functions state machine to be triggered by new images being uploaded to the S3 bucket.
Once you have completed these steps, your serverless image processing application will be ready to use.

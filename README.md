# Ultimate Shell Scripting Project
This project demonstrates how to use shell scripting to automate the management of files in an S3 bucket, and how to trigger a Lambda function in response to S3 events using AWS CLI.


## Features
- Upload files to S3 bucket
- Trigger Lambda function in response to S3 events

## Technologies
- Shell scripting (Bash)
- AWS CLI
- AWS Lambda
- AWS S3

## Prerequisites
- AWS CLI installed and configured with access keys
- AWS Lambda function created and configured to process S3 events
- S3 bucket created and configured with bucket policy and event notifications

## How it Works
The shell script `s3-notification-triggers.sh` provides a menu-driven interface to upload, files in an S3 bucket. It uses the AWS CLI to interact with the S3 bucket.

The script also defines a function `s3-lambda-function.py` that triggers an AWS Lambda function in response to an S3 event. The function uses the AWS CLI to publish a notification to an SNS topic, which in turn triggers the Lambda function.

The Lambda function is configured to process S3 events and perform a specific action based on the event type. For example, if the event type is "object created," the Lambda function can process the uploaded file and perform additional processing or trigger another action.

## Conclusion
The ULTIMATE SHELL SCRIPTING PROJECT demonstrates how to use shell scripting and AWS services to automate the management of files in an S3 bucket and trigger a Lambda function in response to S3 events. This project can be extended to handle more complex use cases and can be a valuable tool for managing files in AWS.

# Deploying-Serverless-Web-Application
Deploying Serverless Web Application on AWS using S3, CloudFront, API Gateway, Lambda Function and DynamoDB

## Architecture
![image](https://github.com/anuragingle01/Hosting-Serverless-Web-Application/assets/110114526/a251464c-1dc1-48aa-80d8-b45ca8315499)

## Steps for Deploying Frontend using CloudFront and S3
### Step 1: Create S3 bucket and add profile.html and scripts.js in bucket
![image](https://github.com/anuragingle01/Hosting-Serverless-Web-Application/assets/110114526/1f280556-9536-4b87-992d-5f8a4f5202b9)

### Step 2: Create distribution in CloudFront and select S3 bucket name as origin domain
![image](https://github.com/anuragingle01/Hosting-Serverless-Web-Application/assets/110114526/019263eb-fd86-48fa-9b01-616f3f6f03fa)

## Steps for Deploying Backend using Lambda Function and DynamoDB
### Step 1: Create two lambda functions getEmployee and insertEmployeeData
Copy lambda function code from getEmployee.py and insertEmployeeData.py and paste into lambda function
![image](https://github.com/anuragingle01/Hosting-Serverless-Web-Application/assets/110114526/2621cff6-992e-4cee-ae9b-0c0513406902)

### Step 2: Create table in DynamoDB with empId as a partition key
![image](https://github.com/anuragingle01/Hosting-Serverless-Web-Application/assets/110114526/ff811ba3-0fca-4934-bda9-bda8827bf27c)

## Steps for API Gateway integration in between CloudFront and Lambda Fuunction
Create RestAPI with two methods get and post 
![image](https://github.com/anuragingle01/Hosting-Serverless-Web-Application/assets/110114526/277a8936-690b-4692-9a3f-18c064988a3f)

## Paste below url in Browser

<a href="https://dae6fbnyzqm4f.cloudfront.net/"> https://dae6fbnyzqm4f.cloudfront.net/

![image](https://github.com/anuragingle01/Hosting-Serverless-Web-Application/assets/110114526/8bd63e05-bfc3-46f1-b6c4-639807c7f7c6)


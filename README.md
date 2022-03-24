# What Is This?
With this repo, you can save your website visitors number on AWS Dynomodb and you can easily expose as api with AWS Lambda Function. İf you want to add visitor number to your website you should use javascript. In this repo, you will learn your website visitors. 

# How Can I Use It?

## Creating Services
First you should create an AWS account. After that you need to create a table named VisitorCount from DynamoDB and partition key must be id(String). 

![image](https://user-images.githubusercontent.com/54737933/159992711-9941e470-5f6b-47d8-b023-465cdb473c89.png)


Than you should edit Item editor like this. After that you should create a Lambda and API Gateway.


## Lambda Function
This repo does not explain AWS setup. If you are having problems about setting up AWS services. Please review the required documents. 

First we are going to write a Lambda Function. Then you will install the `lamda_fuction.py`. Import or copy everything like this.

![image](https://user-images.githubusercontent.com/54737933/159993039-5b51c5e4-d3fa-4b9f-9c1b-3a35b7190cad.png)


After that create a Get Method in API Gateway. Connect the API Gateway with DynamoDB. After that you should Deploy API and Enable CORS.

![image](https://user-images.githubusercontent.com/54737933/159993769-c25b0b3b-7a00-4250-a3e6-0869f670e09d.png)

If you're making the right adjustments, you need this building.


## Usage of Javascript



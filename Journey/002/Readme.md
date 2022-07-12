# LES01-AWS200 - Create a Serverless API

## Introduction



## Prerequisite

This tutorial assumes that you have some knowledge of basic Lambda operations and the Lambda console. If you haven't already, follow the instructions in Create a Lambda function with the console to create your first Lambda function.


## Cloud Research

[Follow this tutorial to understand more about Lambda with API Gateway](https://docs.aws.amazon.com/lambda/latest/dg/services-apigateway-tutorial.html)

## Try yourself

✍️ Add a mini tutorial to encourage the reader to get started learning something new about the cloud.

### Step 1 — Create Lambda Function with basic configuration and choose a language per your choice.

![image](https://user-images.githubusercontent.com/26384517/178560600-0da98e4e-ece3-46e1-83c9-14d997cc610d.png)

### Step 2 — Click on add trigger and it will display new page to configure the other services that you want in our case it is API Gateway

![image](https://user-images.githubusercontent.com/26384517/178560899-9b7bf6e5-a2c1-4950-a146-99dbd7231059.png)

### Step 3 — Select API Gateway in Trigger Configuration and it will show other options to choose

![image](https://user-images.githubusercontent.com/26384517/178561166-4cfb25d2-b79c-4681-9aa3-a228f77007a0.png)

Without API Key no one can access the API.

### Step 4 — Open API Gateway Service Copy Invoke URL

![image](https://user-images.githubusercontent.com/26384517/178562595-ecfa211b-6351-4e7e-b342-31e798d70c03.png)

### Step 5 — Open Postman clinet and paste the URL in Request URL and invoke Get request

![image](https://user-images.githubusercontent.com/26384517/178562926-d8aec505-34dd-44b7-a029-9aeb82b44d6d.png)

you will get the above error as you have not added the API key in postman, without API no one can invoke the API, so where can we find this API key?

### Step 6 — Get API key

![image](https://user-images.githubusercontent.com/26384517/178563782-f0ccc0be-a131-4cbb-b1ee-7f8b2849e80e.png)

### Step 7 — Paste the API key in Postman and Invoke the request

![image](https://user-images.githubusercontent.com/26384517/178564713-0939242c-2ae2-4c4d-8031-29988efd69fc.png)

![image](https://user-images.githubusercontent.com/26384517/178564893-a1b8cc1c-edfd-48f0-b75b-ba9be99edde8.png)

### Step 8 — you can modify the reponse in Lambda function code
![image](https://user-images.githubusercontent.com/26384517/178565196-a2f53d32-4f58-45d4-bec0-156ea421fdf5.png)


## ☁️ Cloud Outcome

Learned how to trigger Lambda function using API Gateway.


## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)

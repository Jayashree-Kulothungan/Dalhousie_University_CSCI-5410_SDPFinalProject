# Dalhousie_University_CSCI-5410_SDPFinalProject

The final project of CSCI 5410 - Serverless Data Processing of MACS at Dalhousie University.

- Project Name : Serverless B&B
- Project Description :
  - The Serverless Bed & Breakfast is a cloud-based hotel reservation system. This system provides the facility to reserve hotel accommodation, order food from the restaurant and allows customers to request a personalized trip package from the tour operator.
- Core components - AWS and GCP services :
  - User Management - AWS Cognito, AWS Lambda, AWS DynamoDB, AWS API Gateway, GCP Firestore
  - Authentication - AWS Cognito, AWS Lambda, AWS DynamoDB, GCP Firestore, GCP Cloud Functions
  - Online Support - AWS S3, AWS Lex, AWS Lambda, AWS Dynamo DB
  - Message Passing - GCP Cloud Functionbs, Pub/Sub, Firestore
  - Machine Learning - GCP NLP API, Vertex AI,
  - Web Application Building and Hosting - React Js, HTML5, CSS, Bootstrap, Material UI, GitLab CI/CD, AWS S3
  - Report Generation - AWS Cloud Trail and AWS CloudWatch
  - Visualization - Google Data Studio
- Team Name : Group no 13
- Team Members :
  - Aditya Deepak Mahale
  - [Jayasree Kulothungan](jayasreekulothungan@gmail.com)
  - Rishika Bajaj
  - Sai Chand Kolloju
  - Sourav Malik
  - Udit Gandhi
- Responsibility
  - User Registration Module
  - Report Generation Module
- Implementation
  - User Registration Module
    - Amazon Cognito : This service is used to store user credentials like email, first name , last name and password. It is also used to verify if email exists.
    - Amazon Lambda : The lambda function is used for 3 purposes – to generate customer Id and to store the credentials in DynamoDB.
    - Amazon DynamoDB : This database service is used to store user credentials like first name, Last name, email, security questions and answers.
    - Amazon API Gateway : This service is used to call the lambda functions that create the customer ID and store data to DynamoDB directly from React.js using REST API.
    - GCP Firestore : This service is used is used to store the email of the user and the secret key provided by them for the purpose of Caesar Cipher.
    - React js, HTML , CSS, Material UI : To create the front-end user registration forms
  - Report Generation Module
    - Amazon CloudTrail : The user logs are maintained the number of logins, registrations and other login details are maintained by integrating AWS CloudTrail. A trail is created that monitors the sign-in and sign-up activities that take place in AWS Cognito
    - Amazon CloudWatch : Reports of Logs from lambda functions, dynamodb and other services can be got from AWS CloudWatch.

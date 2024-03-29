# Exploring-AWS-Image-Recognition-for-Visual-Insights-in-the-Cloud
TITLE OF THE PROJECT:

Exploring AWS Image Recognition for Visual Insights in the Cloud

OBJECTIVE:

To develop a comprehensive understanding of AWS image recognition services, specifically Amazon Rekognition, and their integration within a serverless architecture. The project aims to showcase the deployment of image recognition functionalities such as object detection, facial recognition, and content moderation through the orchestration of Lambda functions, S3 buckets, IAM roles, and API Gateway. By demonstrating the practical applications of these services across diverse use cases, the project seeks to highlight their potential in enhancing various applications and workflows.

DESCRIPTION:

This project explores the potential of Amazon Web Services (AWS) image recognition services for extracting insights from visual data in the cloud. Utilizing tools like Amazon Rekognition and AWS Lambda, we demonstrate various use cases including object detection, facial recognition, and content moderation. Through the integration of AWS Lambda and DynamoDB, data is efficiently managed and processed, with data retrieval facilitated by API Gateway. We address considerations such as cost, scalability, performance, and privacy, providing insights into optimizing serverless architecture and managing DynamoDB capacity. Best practices for deploying image recognition models using AWS services are outlined, offering a comprehensive guide for leveraging AWS image recognition to drive innovation and enhance decision-making processes in the digital era.

ARCHITECTURE:

![image](https://github.com/Mukesh-217/Exploring-AWS-Image-Recognition-for-Visual-Insights-in-the-Cloud/assets/111958305/af809943-46ff-43ed-818d-21c56ca50049)

SERVERLESS SERVICES UTILIZED:

1.Amazon S3: Amazon Simple Storage Service (Amazon S3) is an object storage service offering industry-leading scalability, data availability, security, and performance.

2.AWS Lambda: Run code without provisioning or managing servers, creating workload-aware cluster scaling logic, maintaining event integrations, or managing runtimes.

3.Amazon DynamoDB: Amazon DynamoDB is a serverless, NoSQL database service that enables you to develop modern applications at any scale.

4.Amazon API Gateway: An API gateway is a component of the app-delivery infrastructure that sits between clients and services and provides centralized handling of API communication between them.




IMPLEMENTATION STEPS:

1.Create two S3 buckets with different names, one for the employees and the other for the visitors.

2.Before creating a Lambda function, create a role with the following permissions:

    Amazon DynamoDB Full Access,
    Amazon S3 Full Access,
    Amazon API Gateway Full Access,
    AWS Lambda Full Access
    
3.Create a Lambda function for employee registration where employees can register. Add a trigger for the S3 employee bucket.

4.Create another Lambda function, employee_authentication, for verifying the image.

5.Create an API Gateway to GET and POST the data.

6.Now, create a React Front-end App for the demonstration.

7.Upload the image from the hosted app on localhost:8080 and then verify whether the person in the image is an employee, visitor, or outsider.


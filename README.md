# OluPay 2.0 

##Project Overview

OluPay 2.0 is a production-style serverless payment processing application built on Amazon Web Services (AWS) as part of the BaseStack Academy Cloud Accelerator Capstone Project.

The solution demonstrates secure, scalable, event-driven cloud architecture using managed AWS services and follows AWS Well-Architected Framework best practices.

---





---

## AWS Services Used

- Amazon VPC
- IAM
- Amazon EC2
- Auto Scaling Group
- Application Load Balancer
- Amazon RDS (MySQL)
- Amazon DynamoDB
- Amazon ElastiCache (Redis)
- Amazon API Gateway (HTTP API)
- AWS Lambda
- Amazon SQS
- Amazon SNS
- Amazon CloudWatch

---

## Serverless Workflow

1. Client sends a payment request to the HTTP API.
2. API Gateway invokes the **ProcessPayment** Lambda function.
3. Payment details are stored in DynamoDB.
4. A notification event is sent to Amazon SQS.
5. The **ProcessPaymentNotification** Lambda processes the queue.
6. Amazon SNS sends an email notification.
7. CloudWatch monitors logs, metrics, dashboards, and alarms.

---

## Security Features

- Least-Privilege IAM Roles
- Private Database Resources
- Security Groups
- CloudWatch Monitoring
- SNS Alerting
- SQS Decoupling
- HTTP API Authentication
- Serverless Architecture

---

## Monitoring & Observability

CloudWatch provides:

- Dashboards
- Metrics
- Log Groups
- Logs Insights
- Alarms
- SNS Notifications

---

## Testing

The application was validated using:

- Lambda Test Events
- HTTP API POST Requests
- DynamoDB Item Verification
- SQS Queue Processing
- SNS Email Notifications
- CloudWatch Logs

---

## Repository Structure

```text
architecture/
lambda/
screenshots/
docs/
```

---

## Author

**ShadowStricker**

BaseStack Academy Cloud Accelerator Programme

AWS Cloud Capstone Project (2026)

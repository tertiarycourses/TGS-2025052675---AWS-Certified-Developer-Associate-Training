# TGS-2025052675 - AWS Certified Developer Associate Training

> Course: AWS Certified Developer Associate Training  
> Course Code: TGS-2025052675  
> Register here: https://www.tertiarycourses.com.sg/wsq-aws-certified-developer-associate-training.html

Hands-on AWS Certified Developer Associate labs for learners preparing for the AWS Certified Developer - Associate exam. The labs cover AWS developer tools, IAM for applications, SDKs, Lambda, API Gateway, DynamoDB, S3, messaging, CI/CD, deployment, monitoring, troubleshooting, security, optimization, and exam-style review.

## Courseware

| Item | Description |
| --- | --- |
| [Learner Guide](LG-AWS-Certified-Developer-Associate-Training.md) | Detailed step-by-step guide for completing the labs and preparing final deliverables. |
| [Lab Guide](labs/README.md) | Lab catalogue grouped by AWS developer skill area. |
| [Tools Reference](labs/tools.md) | Recommended AWS tools, free tier notes, and learner setup checklist. |

## How to Use

1. Create or use an AWS account provided by your trainer.
2. Create a working folder named `TGS-2025052675-AWS-DVA-Labs`.
3. Complete the labs in sequence because later labs reuse IAM, Lambda, API Gateway, DynamoDB, monitoring, and deployment concepts.
4. Record screenshots, commands, code snippets, and configuration notes for each lab.
5. Delete paid resources when the lab asks you to clean up.

## Lab Catalogue

### Domain 1 - Developer Foundations and Serverless Applications

| Lab | Title | Focus |
| --- | --- | --- |
| [Lab 1](labs/lab-01-account-iam-cli-sdk-developer-setup.md) | Account Safety, IAM, AWS CLI, SDKs, and Developer Setup | MFA, IAM roles, access keys, AWS CLI, SDK configuration, CloudShell |
| [Lab 2](labs/lab-02-lambda-api-gateway-serverless-api.md) | Lambda, API Gateway, and Serverless APIs | Lambda functions, triggers, API Gateway routes, permissions, testing |
| [Lab 3](labs/lab-03-dynamodb-s3-application-data.md) | DynamoDB, S3, and Application Data Patterns | DynamoDB keys, indexes, S3 object access, presigned URLs, data patterns |

### Domain 2 - Event-Driven Development and CI/CD

| Lab | Title | Focus |
| --- | --- | --- |
| [Lab 4](labs/lab-04-sqs-sns-eventbridge-step-functions.md) | SQS, SNS, EventBridge, and Step Functions | Queues, topics, event rules, workflow orchestration, retries, DLQs |
| [Lab 5](labs/lab-05-codecommit-codebuild-codedeploy-codepipeline.md) | Developer Tools and CI/CD Pipelines | Source, build, test, deploy, CodePipeline, CodeBuild, CodeDeploy concepts |
| [Lab 6](labs/lab-06-deployment-sam-cloudformation-containers.md) | Deployment with SAM, CloudFormation, Elastic Beanstalk, and Containers | IaC, SAM templates, CloudFormation stacks, Elastic Beanstalk, ECS/ECR |

### Domain 3 - Security, Monitoring, Optimization, and Exam Review

| Lab | Title | Focus |
| --- | --- | --- |
| [Lab 7](labs/lab-07-security-secrets-cognito-kms.md) | Application Security, Secrets, Cognito, KMS, and Least Privilege | Secrets Manager, Parameter Store, Cognito, KMS, IAM policies, encryption |
| [Lab 8](labs/lab-08-monitoring-troubleshooting-optimization-exam-review.md) | Monitoring, Troubleshooting, Optimization, and Exam Review | CloudWatch, X-Ray, CloudTrail, logs, metrics, alarms, caching, throttling, timed practice |

## Reference

- AWS Certified Developer - Associate: https://aws.amazon.com/certification/certified-developer-associate/
- Course registration: https://www.tertiarycourses.com.sg/wsq-aws-certified-developer-associate-training.html
- AWS Documentation: https://docs.aws.amazon.com/
- AWS Skill Builder: https://skillbuilder.aws/

## Free Tools Used

- AWS Free Tier eligible services where possible
- AWS Management Console
- AWS CloudShell
- AWS CLI
- AWS SDKs
- AWS SAM CLI
- Amazon CloudWatch
- AWS Pricing Calculator

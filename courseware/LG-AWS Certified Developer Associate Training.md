# Learner Guide - AWS Certified Developer Associate Training

**TGS Ref No:** TGS-2025052675
**Provider:** Tertiary Infotech Academy Pte Ltd (UEN: 201200696W)
**Version:** 3

This Markdown file mirrors the Learner Guide and follows the authoritative labs in exact order.

## Lab Alignment Matrix

| Lab | Capability | Source |
| --- | --- | --- |
| 1 - Account Safety, IAM, AWS CLI, SDKs, and Developer Setup | Domain 1 - Development with AWS Services | `lab-01-account-iam-cli-sdk-developer-setup.md` |
| 2 - Lambda, API Gateway, and Serverless APIs | Domain 1 - Development with AWS Services | `lab-02-lambda-api-gateway-serverless-api.md` |
| 3 - DynamoDB, S3, and Application Data Patterns | Domain 1 - Development with AWS Services | `lab-03-dynamodb-s3-application-data.md` |
| 4 - SQS, SNS, EventBridge, and Step Functions | Domain 2 - Security and Deployment | `lab-04-sqs-sns-eventbridge-step-functions.md` |
| 5 - Developer Tools and CI/CD Pipelines | Domain 2 - Security and Deployment | `lab-05-codecommit-codebuild-codedeploy-codepipeline.md` |
| 6 - Deployment with SAM, CloudFormation, Elastic Beanstalk, and Containers | Domain 2 - Security and Deployment | `lab-06-deployment-sam-cloudformation-containers.md` |
| 7 - Application Security, Secrets, Cognito, KMS, and Least Privilege | Domain 3 - Troubleshooting and Optimization | `lab-07-security-secrets-cognito-kms.md` |
| 8 - Monitoring, Troubleshooting, Optimization, and Exam Review | Domain 3 - Troubleshooting and Optimization | `lab-08-monitoring-troubleshooting-optimization-exam-review.md` |

# Lab 1 - Account Safety, IAM, AWS CLI, SDKs, and Developer Setup

**Day:** 1  
**Capability:** Domain 1 - Development with AWS Services  
**Authoritative source:** `lab-01-account-iam-cli-sdk-developer-setup.md`

## Lab 1 - Account Safety, IAM, AWS CLI, SDKs, and Developer Setup

## Objectives

- Configure a safe AWS developer baseline.
- Review IAM users, roles, policies, and least privilege.
- Use AWS CloudShell or AWS CLI.
- Understand SDK configuration and credential safety.

## Scenario

AWS developers need secure access to services and tooling before building applications. This lab establishes a safe setup and reviews how applications authenticate to AWS.

## Steps

1. Sign in to the AWS account assigned by your trainer.
2. Confirm you are in the correct region.
3. Open IAM.
4. Verify MFA is enabled where permitted.
5. Review users, groups, roles, and policies.
6. Open an AWS managed policy and identify actions, resources, and effects.
7. Create or review a developer role only if your trainer permits it.
8. Open AWS CloudShell.
9. Run `aws sts get-caller-identity`.
10. Run `aws configure list`.
11. Review the difference between access keys, temporary credentials, roles, and instance profiles.
12. Open AWS SDK documentation for one language such as Python, JavaScript, Java, or .NET.
13. Record how the SDK credential provider chain works at a high level.
14. Create a short least-privilege checklist for application development.
15. Save your notes.

## Deliverables

- IAM concept notes
- CloudShell command output notes
- Credential safety checklist
- SDK configuration notes

## Checkpoint

You should be able to explain how developers and applications authenticate to AWS securely.


# Lab 2 - Lambda, API Gateway, and Serverless APIs

**Day:** 1  
**Capability:** Domain 1 - Development with AWS Services  
**Authoritative source:** `lab-02-lambda-api-gateway-serverless-api.md`

## Lab 2 - Lambda, API Gateway, and Serverless APIs

## Objectives

- Understand Lambda function configuration.
- Create or review a Lambda test event.
- Connect Lambda to API Gateway conceptually or hands-on if permitted.
- Review permissions, logs, timeout, memory, and versions.

## Scenario

Serverless APIs are common on AWS. You will design a small API workflow and learn the key configuration points tested in AWS Developer Associate scenarios.

## Steps

1. Open AWS Lambda.
2. Create a function only if your trainer permits it.
3. Choose an approved runtime such as Python or Node.js.
4. Review handler, runtime, timeout, memory, environment variables, and execution role.
5. Create a test event.
6. Run the test event and review the response.
7. Open CloudWatch Logs for the function.
8. Add or review a simple log statement.
9. Review function versions and aliases.
10. Review concurrency and throttling concepts.
11. Open API Gateway.
12. Review REST API, HTTP API, routes, stages, integrations, and authorizers.
13. Create a simple route to Lambda only if permitted.
14. Test the route or document the request/response flow.
15. Review Lambda resource-based permissions for API Gateway invocation.
16. Delete any test API and function if instructed.
17. Save your notes.

## Deliverables

- Lambda configuration notes
- Test event notes
- API Gateway request flow notes
- CloudWatch log notes

## Checkpoint

You should be able to explain how API Gateway invokes Lambda and where to troubleshoot function errors.


# Lab 3 - DynamoDB, S3, and Application Data Patterns

**Day:** 1  
**Capability:** Domain 1 - Development with AWS Services  
**Authoritative source:** `lab-03-dynamodb-s3-application-data.md`

## Lab 3 - DynamoDB, S3, and Application Data Patterns

## Objectives

- Model application data using DynamoDB access patterns.
- Review keys, indexes, capacity, TTL, and streams.
- Understand S3 object access and presigned URLs.
- Compare data storage choices for applications.

## Scenario

Applications commonly use DynamoDB for low-latency key-value access and S3 for object storage. You will review both services from a developer perspective.

## Steps

1. Open DynamoDB.
2. Review table, partition key, sort key, item, and attribute concepts.
3. Create a table only if your trainer permits it.
4. Choose a sample access pattern such as `Get order by order_id`.
5. Add a sample item if permitted.
6. Review global secondary index and local secondary index concepts.
7. Review capacity modes and throttling behavior.
8. Review TTL and DynamoDB Streams use cases.
9. Open S3.
10. Review bucket, object, prefix, metadata, and versioning concepts.
11. Create a bucket only if permitted.
12. Keep Block Public Access enabled.
13. Upload a small sample file if permitted.
14. Review presigned URL use cases.
15. Create a table comparing DynamoDB, S3, RDS, and ElastiCache for application data.
16. Delete temporary resources if instructed.
17. Save your notes.

## Deliverables

- DynamoDB access pattern notes
- Key and index design notes
- S3 object access notes
- Application data service comparison table

## Checkpoint

You should be able to choose application data services based on latency, access pattern, object storage, and caching needs.


# Lab 4 - SQS, SNS, EventBridge, and Step Functions

**Day:** 1  
**Capability:** Domain 2 - Security and Deployment  
**Authoritative source:** `lab-04-sqs-sns-eventbridge-step-functions.md`

## Lab 4 - SQS, SNS, EventBridge, and Step Functions

## Objectives

- Compare asynchronous messaging and event services.
- Understand queues, topics, event buses, and workflows.
- Design retry and dead-letter queue behavior.
- Map event-driven services to application scenarios.

## Scenario

AWS applications often decouple components with queues, topics, events, and workflows. This lab helps you choose the right event-driven service.

## Steps

1. Open Amazon SQS.
2. Review standard and FIFO queue concepts.
3. Review visibility timeout, message retention, long polling, and dead-letter queues.
4. Open Amazon SNS.
5. Review topics, subscriptions, fanout, and filtering.
6. Open Amazon EventBridge.
7. Review event buses, rules, schedules, and targets.
8. Open AWS Step Functions.
9. Review state machines, tasks, choices, retries, catches, and executions.
10. Create a comparison table for SQS, SNS, EventBridge, and Step Functions.
11. Design a workflow where an API request queues work for a background processor.
12. Add retry and DLQ handling.
13. Design a fanout notification pattern.
14. Design a scheduled event pattern.
15. Save your notes.

## Deliverables

- Event service comparison table
- Queue-based processing design
- Fanout design
- Retry and DLQ notes

## Checkpoint

You should be able to match SQS, SNS, EventBridge, and Step Functions to common application integration scenarios.


# Lab 5 - Developer Tools and CI/CD Pipelines

**Day:** 2  
**Capability:** Domain 2 - Security and Deployment  
**Authoritative source:** `lab-05-codecommit-codebuild-codedeploy-codepipeline.md`

## Lab 5 - Developer Tools and CI/CD Pipelines

## Objectives

- Understand AWS developer tools for CI/CD.
- Review source, build, test, deploy, and release stages.
- Compare CodeCommit, CodeBuild, CodeDeploy, and CodePipeline.
- Design a simple application delivery pipeline.

## Scenario

The AWS Developer Associate exam expects knowledge of packaging, deploying, and automating releases. You will design a CI/CD pipeline and identify where build artifacts and deployment strategies fit.

## Steps

1. Open CodePipeline.
2. Review pipeline stages and actions.
3. Open CodeBuild.
4. Review build projects, buildspec files, environment images, artifacts, and logs.
5. Open CodeDeploy.
6. Review deployment groups, deployment configurations, lifecycle hooks, and rollback concepts.
7. Open CodeCommit if available or use a trainer-approved external Git provider.
8. Create a comparison table for source, build, deploy, and pipeline services.
9. Design a pipeline with source, build, test, package, deploy, and approval stages.
10. Identify where artifacts are stored.
11. Identify where environment variables and secrets should be handled.
12. Compare blue/green, rolling, canary, and all-at-once deployment concepts.
13. Review failure and rollback paths.
14. Save your pipeline design.

## Deliverables

- CI/CD service comparison table
- Pipeline design
- Deployment strategy notes
- Rollback and artifact notes

## Checkpoint

You should be able to explain how AWS developer tools automate build, test, deployment, and rollback workflows.


# Lab 6 - Deployment with SAM, CloudFormation, Elastic Beanstalk, and Containers

**Day:** 2  
**Capability:** Domain 2 - Security and Deployment  
**Authoritative source:** `lab-06-deployment-sam-cloudformation-containers.md`

## Lab 6 - Deployment with SAM, CloudFormation, Elastic Beanstalk, and Containers

## Objectives

- Compare AWS deployment and infrastructure-as-code options.
- Understand CloudFormation templates and stacks.
- Review AWS SAM for serverless deployment.
- Compare Elastic Beanstalk and container deployment patterns.

## Scenario

Developers must package and deploy applications consistently. This lab reviews deployment tools and when each option is appropriate.

## Steps

1. Open CloudFormation.
2. Review stacks, templates, parameters, outputs, change sets, and drift detection.
3. Open AWS SAM documentation or service pages.
4. Review the purpose of `template.yaml`, functions, APIs, and permissions.
5. Review SAM build, package, deploy, and local testing concepts.
6. Open Elastic Beanstalk.
7. Review environments, application versions, platforms, and deployment policies.
8. Open Amazon ECR.
9. Review container image repository concepts.
10. Open ECS.
11. Review clusters, task definitions, services, and tasks.
12. Create a comparison table for CloudFormation, SAM, Elastic Beanstalk, ECS, and Lambda console deployment.
13. Design a deployment path for a small serverless API.
14. Design a deployment path for a containerized web application.
15. Save your notes.

## Deliverables

- Deployment service comparison table
- Serverless deployment design
- Container deployment design
- CloudFormation and SAM notes

## Checkpoint

You should be able to explain how AWS applications are packaged and deployed using infrastructure-as-code and managed deployment services.


# Lab 7 - Application Security, Secrets, Cognito, KMS, and Least Privilege

**Day:** 2  
**Capability:** Domain 3 - Troubleshooting and Optimization  
**Authoritative source:** `lab-07-security-secrets-cognito-kms.md`

## Lab 7 - Application Security, Secrets, Cognito, KMS, and Least Privilege

## Objectives

- Secure application secrets and configuration.
- Review Cognito authentication and authorization patterns.
- Understand KMS encryption for application data.
- Apply least-privilege and resource-based permissions.

## Scenario

Application security is central to AWS development. You will review identity, secrets, encryption, and permission patterns that commonly appear in exam scenarios.

## Steps

1. Open Secrets Manager.
2. Review secret storage, rotation, versions, and access policies.
3. Open Systems Manager Parameter Store.
4. Compare standard parameters, secure strings, and hierarchy naming.
5. Open Amazon Cognito.
6. Review user pools, identity pools, app clients, and hosted UI concepts.
7. Open KMS.
8. Review AWS managed keys, customer managed keys, key policies, and grants.
9. Review Lambda environment variable encryption.
10. Review IAM identity-based policies and resource-based policies.
11. Compare API Gateway IAM authorization, Lambda authorizers, and Cognito authorizers.
12. Create a secure application checklist.
13. Map where secrets, config, tokens, encryption keys, and permissions belong in an application.
14. Save your notes.

## Deliverables

- Secrets Manager vs Parameter Store comparison
- Cognito concept notes
- KMS encryption notes
- Secure application checklist

## Checkpoint

You should be able to explain how AWS applications manage secrets, user identity, encryption, and least-privilege permissions.


# Lab 8 - Monitoring, Troubleshooting, Optimization, and Exam Review

**Day:** 2  
**Capability:** Domain 3 - Troubleshooting and Optimization  
**Authoritative source:** `lab-08-monitoring-troubleshooting-optimization-exam-review.md`

## Lab 8 - Monitoring, Troubleshooting, Optimization, and Exam Review

## Objectives

- Review application observability tools.
- Diagnose common Lambda, API Gateway, DynamoDB, and deployment issues.
- Identify performance and cost optimization patterns.
- Complete certification-style review practice.

## Scenario

The final lab ties together debugging, observability, optimization, and exam readiness for AWS developer workloads.

## Steps

1. Open CloudWatch.
2. Review metrics, logs, log groups, dashboards, and alarms.
3. Review Lambda logs and metrics such as errors, duration, throttles, and concurrent executions.
4. Review API Gateway metrics and access logs conceptually.
5. Open X-Ray.
6. Review traces, segments, service maps, and sampling concepts.
7. Open CloudTrail and review audit events.
8. Create a troubleshooting checklist for Lambda permission errors, timeout errors, throttling, API errors, and DynamoDB throttling.
9. Create an optimization checklist covering memory tuning, retries with backoff, caching, connection reuse, SDK pagination, and reserved concurrency.
10. Review DAX, ElastiCache, CloudFront, and API Gateway caching use cases.
11. Map each lab to exam domains.
12. Complete a timed 30-question practice set from trainer-provided questions or AWS practice resources.
13. Mark weak topics by domain.
14. Clean up temporary resources if instructed.
15. Save final notes.

## Deliverables

- Monitoring and troubleshooting checklist
- Optimization checklist
- Exam-domain revision map
- Timed practice score
- Weak-topic revision plan

## Checkpoint

You should be ready to explain AWS developer services, application deployment, security, troubleshooting, and optimization under exam-style scenarios.


# Support and Assessment Flow

Courseware and assessment: https://lms-tms.tertiaryinfotech.com/

1. Complete TRAQOM digital attendance.
2. Complete Assessment Digital Attendance.
3. Sit the Written Assessment and Practical Performance assessment.
4. Submit answers on the LMS.
5. Sign the Assessment Summary Record.
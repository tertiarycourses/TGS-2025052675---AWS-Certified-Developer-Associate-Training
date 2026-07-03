# Learner Guide - AWS Certified Developer Associate Training

> Course: AWS Certified Developer Associate Training  
> Course Code: TGS-2025052675  
> Registration: https://www.tertiarycourses.com.sg/wsq-aws-certified-developer-associate-training.html

This learner guide supports a practical AWS Certified Developer Associate course. It is designed for learners preparing to develop, test, deploy, optimize, package, monitor, and troubleshoot AWS cloud-based applications.

## Learning Outcomes

By the end of the labs, you should be able to:

- Configure a secure AWS developer setup using IAM, CLI, SDKs, and CloudShell.
- Build and troubleshoot serverless APIs using Lambda and API Gateway.
- Design application data access patterns with DynamoDB, S3, RDS, and caching services.
- Use event-driven services such as SQS, SNS, EventBridge, and Step Functions.
- Design CI/CD pipelines using AWS developer tools and deployment strategies.
- Compare deployment options such as CloudFormation, SAM, Elastic Beanstalk, Lambda, and containers.
- Secure applications using Secrets Manager, Parameter Store, Cognito, KMS, IAM, and resource policies.
- Monitor, troubleshoot, and optimize applications using CloudWatch, X-Ray, CloudTrail, caching, retries, and throttling controls.
- Prepare for exam-style AWS Developer Associate scenario questions.

## Recommended Setup

1. Use a trainer-provided AWS account where available.
2. If using your own account, enable MFA and create a budget alert before starting labs.
3. Create a working folder named `TGS-2025052675-AWS-DVA-Labs`.
4. Save screenshots, commands, snippets, architecture notes, and comparison tables.
5. Delete temporary AWS resources after each hands-on exercise.

## Cost Safety Rules

- Use small test functions and sample data.
- Avoid long-running compute, provisioned capacity, and repeated build minutes unless explicitly assigned.
- Delete test APIs, Lambda functions, queues, topics, stacks, build projects, and buckets after labs if instructed.
- Check Billing and Cost Management after hands-on labs.

## Lab 1 - Account Safety, IAM, AWS CLI, SDKs, and Developer Setup

### Objectives

- Establish a secure AWS developer baseline.
- Review IAM and credential safety.
- Use AWS CloudShell or CLI.
- Understand SDK configuration.

### Procedure

1. Sign in to the assigned AWS account.
2. Confirm account and region.
3. Open IAM and review users, groups, roles, and policies.
4. Verify MFA where permitted.
5. Review an AWS managed policy.
6. Open CloudShell.
7. Run `aws sts get-caller-identity`.
8. Run `aws configure list`.
9. Compare access keys, temporary credentials, roles, and instance profiles.
10. Review one AWS SDK credential provider chain.
11. Create a least-privilege checklist.
12. Save your notes.

### Checkpoint

You should be able to explain secure developer authentication and application credential patterns.

## Lab 2 - Lambda, API Gateway, and Serverless APIs

### Objectives

- Review Lambda configuration.
- Test Lambda events.
- Understand API Gateway integration.
- Troubleshoot logs and permissions.

### Procedure

1. Open Lambda.
2. Create a small test function only if permitted.
3. Review handler, runtime, timeout, memory, environment variables, and execution role.
4. Create and run a test event.
5. Review CloudWatch Logs.
6. Review versions, aliases, concurrency, and throttling.
7. Open API Gateway.
8. Review REST API, HTTP API, routes, stages, integrations, and authorizers.
9. Connect API Gateway to Lambda only if permitted.
10. Review Lambda resource-based permissions.
11. Delete test resources if instructed.
12. Save your notes.

### Checkpoint

You should be able to explain API Gateway to Lambda request flow and troubleshooting points.

## Lab 3 - DynamoDB, S3, and Application Data Patterns

### Objectives

- Design DynamoDB access patterns.
- Review S3 object access.
- Compare application data services.
- Understand throttling and indexing concepts.

### Procedure

1. Open DynamoDB.
2. Review table, partition key, sort key, item, and attribute concepts.
3. Create a table only if permitted.
4. Define a sample access pattern.
5. Review GSI, LSI, capacity modes, TTL, and streams.
6. Open S3.
7. Review buckets, objects, prefixes, metadata, and versioning.
8. Review presigned URL use cases.
9. Compare DynamoDB, S3, RDS, and ElastiCache.
10. Delete temporary resources if instructed.
11. Save your notes.

### Checkpoint

You should be able to choose application data services based on access pattern and storage requirements.

## Lab 4 - SQS, SNS, EventBridge, and Step Functions

### Objectives

- Compare event-driven services.
- Design asynchronous workflows.
- Add retry and dead-letter behavior.
- Match services to scenarios.

### Procedure

1. Review SQS standard and FIFO queue concepts.
2. Review visibility timeout, retention, long polling, and dead-letter queues.
3. Review SNS topics, subscriptions, fanout, and filtering.
4. Review EventBridge event buses, rules, schedules, and targets.
5. Review Step Functions state machines, retries, catches, and executions.
6. Create a comparison table.
7. Design a queue-based background processor.
8. Design a fanout notification pattern.
9. Design a scheduled event pattern.
10. Save your notes.

### Checkpoint

You should be able to choose SQS, SNS, EventBridge, or Step Functions for common application integration scenarios.

## Lab 5 - Developer Tools and CI/CD Pipelines

### Objectives

- Understand CI/CD stages.
- Compare AWS developer tools.
- Design a pipeline.
- Review deployment strategies and rollback.

### Procedure

1. Review CodePipeline stages and actions.
2. Review CodeBuild buildspec, environment, artifacts, and logs.
3. Review CodeDeploy deployment groups, lifecycle hooks, and rollback.
4. Review CodeCommit or an external Git source option.
5. Create a source-build-test-deploy pipeline design.
6. Identify artifact storage.
7. Identify secret and environment variable handling.
8. Compare blue/green, rolling, canary, and all-at-once deployments.
9. Save your notes.

### Checkpoint

You should be able to explain build, package, deploy, approval, and rollback workflows.

## Lab 6 - Deployment with SAM, CloudFormation, Elastic Beanstalk, and Containers

### Objectives

- Compare deployment tools.
- Understand infrastructure as code.
- Review SAM and CloudFormation concepts.
- Compare managed application and container deployment.

### Procedure

1. Review CloudFormation stacks, templates, parameters, outputs, change sets, and drift detection.
2. Review SAM templates, functions, APIs, permissions, build, package, and deploy concepts.
3. Review Elastic Beanstalk applications and environments.
4. Review ECR repositories and ECS task/service concepts.
5. Create a deployment service comparison table.
6. Design deployment for a serverless API.
7. Design deployment for a containerized web application.
8. Save your notes.

### Checkpoint

You should be able to explain AWS deployment choices for common developer workloads.

## Lab 7 - Application Security, Secrets, Cognito, KMS, and Least Privilege

### Objectives

- Secure secrets and configuration.
- Review user authentication services.
- Understand encryption and IAM policies.
- Build a secure application checklist.

### Procedure

1. Review Secrets Manager.
2. Review Parameter Store.
3. Compare secret rotation, secure strings, and configuration hierarchies.
4. Review Cognito user pools and identity pools.
5. Review KMS keys, key policies, and grants.
6. Review Lambda environment variable encryption.
7. Compare IAM identity-based and resource-based policies.
8. Compare API Gateway IAM, Lambda authorizers, and Cognito authorizers.
9. Create a secure application checklist.
10. Save your notes.

### Checkpoint

You should be able to explain application secrets, identity, encryption, and least-privilege design.

## Lab 8 - Monitoring, Troubleshooting, Optimization, and Exam Review

### Objectives

- Review observability and debugging tools.
- Diagnose common developer issues.
- Identify optimization patterns.
- Complete timed practice.

### Procedure

1. Review CloudWatch metrics, logs, dashboards, and alarms.
2. Review Lambda errors, duration, throttles, and concurrency metrics.
3. Review API Gateway metrics and access log concepts.
4. Review X-Ray traces and service maps.
5. Review CloudTrail audit events.
6. Create a troubleshooting checklist for permission errors, timeouts, throttling, API errors, and DynamoDB throttling.
7. Create an optimization checklist covering memory tuning, retries with backoff, caching, connection reuse, SDK pagination, and reserved concurrency.
8. Review DAX, ElastiCache, CloudFront, and API Gateway caching use cases.
9. Complete a timed 30-question practice set.
10. Mark weak topics and create a revision plan.
11. Clean up temporary resources.

### Checkpoint

You should be ready to explain AWS developer services, deployment, security, troubleshooting, and optimization under exam conditions.

## Final Submission Checklist

- Lab notes or screenshots
- CLI and SDK notes
- Serverless API and event-driven architecture notes
- CI/CD and deployment comparison tables
- Security checklist
- Monitoring and troubleshooting checklist
- Timed practice score
- Weak-topic revision plan

## Suggested Course Flow

| Segment | Focus | Labs |
| --- | --- | --- |
| Segment 1 | Developer setup, IAM, Lambda, API Gateway, app data | Labs 1-3 |
| Segment 2 | Event-driven development, CI/CD, deployment | Labs 4-6 |
| Segment 3 | Security, monitoring, troubleshooting, exam review | Labs 7-8 |

## Clean Up

1. Delete temporary Lambda functions, APIs, queues, topics, and state machines if instructed.
2. Delete temporary S3 buckets, DynamoDB tables, build projects, stacks, and test resources if instructed.
3. Stop or delete any provisioned resources that may incur cost.
4. Keep budget alerts active until the trainer confirms cleanup.
5. Save notes for final revision.

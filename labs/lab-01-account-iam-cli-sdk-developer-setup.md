# Lab 1 - Account Safety, IAM, AWS CLI, SDKs, and Developer Setup

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

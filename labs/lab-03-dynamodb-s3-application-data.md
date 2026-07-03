# Lab 3 - DynamoDB, S3, and Application Data Patterns

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

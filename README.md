## Automated Data Pipeline Using Lambda, S3 and Glue

The steps included:
1. Create two S3 buckets: one is the source bucket, which has the JSON files, and the other is the destination bucket, which flattens into CSV format
2. Create an IAM role for AWS Lambda function, which is triggered when a new JSON file gets uploaded into the S3 source bucket (CloudWatch, S3, Glue permission)
3. Now, we create a Lambda function (in Python) and add the respective trigger
4. Create an IAM role for the Glue Job (CloudWatch, S3 full access)
5. Then, create a Glue Job using the AWS service AWS Glue
6. Set up the environment and now upload a JSON file into the S3 Source bucket
7. If we now check the destination bucket, we find that the JSON file has been flattened out to a CSV file
8. Time to clean up!

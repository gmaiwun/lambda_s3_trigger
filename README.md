# lambda_s3_trigger
To create a Lambda function that is triggered when a .csv file is uploaded in an s3 bucket, scans the content of the file, uploads this content to an RDS Mysql database. Some things to note for this exercise are as follows:

- *Make sure the database credentials are **NOT** hard-coded into the Lambda function*
- *For this exercise, i have **NOT** constrained the Lambda function to the same VPC as the RDS database. So, for this to work, you should ensure that the database is publicly accessible. (You can extend this exercise by exploring a scenario where the Lambda function is in the same VPC as the database and other utilized resources)*

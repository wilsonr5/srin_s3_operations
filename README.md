# srin_s3_operations
AWS S3 Operations Demonstration
This repo include all the sample files that is used for AWS S3 operations that is located in a directory named Files.

# Create bucket
aws s3 mb s3://<bucket_name> [--options]

# Delete bucket
aws s3 rb s3://<bucket_name> [--options]

# List buckets
aws s3 ls [s3://<bucket_name>] [--options]

# Create Object
aws s3api put-object --bucket <bucket_name> --key <bucket_path> [--options]

# Update Object
aws s3api put-object --bucket <bucket_name> --key <bucket_path> --body <local_path> [--options]
aws s3 sync <local_path> s3://<bucket_path> [--options]

# Delete Object
aws s3api delete-object --bucket <bucket_name> --key <bucket_path> [--options]

# List Objects in Specified Bucket and Sub-bucket
aws s3 ls s3://<bucket_name> --recursive [--options]

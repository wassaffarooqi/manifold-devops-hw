# manifold-devops-hw

## Homework Problem

### BACKGROUND

Our goal is to build an endpoint for a hypothetical vendor to send us user data in slightly different formats; The design is in place but needs to be automated.

### Assignment

Please support the Dev Team,  produce the Terraform code needed to support a Dev Team tasked with the following below.  This will include documentation on what is created, and any other support documentation you feel someone would need as a user of this code.  

The dev team assignment calls for a python code, supplied is a stub file.  The stub file is fine to use for the Lambda function. OPTIONAL: build out the stub file and write testing.

### Dev Teams Assignment needing support

Please make an API endpoint deployed on AWS that will take in a JSON data structure. From inside the structure, it should pull out first_name, middle_name, last_name, and zip_code, and store that data in S3.

Make this using API Gateway and Lambda (with python code).

After the data is stored in S3, make a queryable table with AWS Glue and be able to present it for querying using Athena. 


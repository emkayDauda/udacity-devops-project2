## Maaruf Dauda - Submission for project Two
This folder contains the templates necessary for creating the infrastructure required for the second project

### Dependencies
##### 1. AWS account
You would be required to have an AWS account to be able to build cloud infrastructure.

##### 2. S3 Bucket
An S3 bucket containing at least, the index.html file to deploy. You may also upload into the bucket, an entire folder of html pages and style files, but ensure the `index.html` file is in the root folder.

##### 3. Terminal
A terminal to run the scripts


### How to run the script and create your infrastructure?
You can run the supporting material in two easy steps:
```bash
# Ensure that the AWS CLI is configured before running the command below
# Create the network infrastructure
# Check the region in the create.sh file
./create.sh udagram-infra final-project-network-infra.yml infra-parameters.json
# Create servers
# Ensure the network-infra template runs successfully and wait until all resources are created
# Update the `server-parameters.json` file. Update it with your bucket name and the appropriate ubuntu v18 image id for your region
# Run the server template
./create.sh udagram final-project.yml server-parameters.json
```
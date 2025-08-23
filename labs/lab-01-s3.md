# Lab 01 - S3 Setup Via Console + CloudShell
## Region We use **us-east-2 (Ohio)** for this lab.
## Steps (CloudShell + CLI)'''bash
aws configure set region us-east-2 aws s3 1s
mkdir -p lab && echo "hello from cloudshell" > lab/hello.txt aws s3 cp lab/hello.txt s3://<jonne-cloud-journey-demo>/hello.txt aws s3 presign s3://<jonne-cloud-journey-demo>/hello.txt --expires-in 3600

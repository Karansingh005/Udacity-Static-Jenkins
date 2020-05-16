# Udacity-Static-Jenkins
This is a repository, containing code for deploying a static web application on Amazon S3 bucket on Amazon Web Services Platform, using Jenkins and BlueOcean. This code was tested to run on Amazon EC2 Ubuntu instance, which is a service by Amazon Web Services. 

## Requirements to deploy the static website using Jenkins
1. Set up an account for Amazon Web Serivces to use services by AWS, to deploy this code on Jenkins. Here's a link to register your own AWS account: [AWS registration portal]('https://portal.aws.amazon.com/billing/signup#/start')
2. Set up an IAM user in AWS console, with permissions for EC2 Full Access, S3 Bucket Full Access and VPC FUll Access. Here's a link to know more about IAM users in AWS: [AWS Documentation: What is IAM?]('https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html')
3. Copy the generated Access Key and Secret Access Key of your IAM user, and login to the console using that. 

## Launch an EC2 instance and install Jenkins on it
1. Set up an EC2 Instance with following parameters: 
* Ubuntu 18.04
* T2.micro
* Security Group: Add Custom TCP Rule, Port Range 8080, Source 0.0.0.0/0 and SSH rule: Protocol: SSH, Port range: 22, Source "My IP"
Here's a link to help in launching EC2 instance: https://docs.aws.amazon.com/quickstarts/latest/vmlaunch/step-1-launch-instance.html

2. Connect to your EC2 instance. Here's a guide to connect to EC2 instance to your local machine: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Connect-using-EC2-Instance-Connect.html

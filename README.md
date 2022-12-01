# infrastructure


## Setup
## Aws cli 
* For setting AWS CLI, Download and run the AWS CLI MSI installer for Windows (64-bit): https://awscli.amazonaws.com/AWSCLIV2.msi 
* set profile for aws accounts

## Build & Deploy
* Clone repository
* Now navigate to script folder using command "cd infrastructure/aws/cloudformation/"
  
* Create a aws cloud formation stack in Default Region
   
    aws cloudformation create-stack --stack-name "Stackname" --template-body "YML Or JSON File" 

* Create a aws cloud formation stack in specified Region
     
     aws cloudformation create-stack --stack-name "Stack Name" --template-body "YML Or JSON File" --region "Region name"

* To delete a cloudformation stack run aws cli command
  
	Delete stack - aws cloudformation delete-stack --stack-name "Stackname"

## Command to import SSL certificate into AWS Certificate Manager

   aws acm import-certificate --certificate fileb://Certificate.pem --private-key fileb://PrivateKey.pem
aws cloudformation create-stack --stack-name mate-workshop --template-body file:///Users/awsric/Documents/aws-pocs/ci-workshop/aws/prerequisites.yml  --tags Key=Example,Value=CIWorkShop --capabilities CAPABILITY_IAM   && aws cloudformation wait stack-create-complete --stack-name mate-workshop


aws cloudformation update-stack --stack-name mate-workshop --template-body file:///Users/awsric/Documents/aws-pocs/ci-workshop/aws/prerequisites.yml  --tags Key=Example,Value=BasicFunctionJava --capabilities CAPABILITY_IAM   && aws cloudformation wait stack-update-complete --stack-name mate-workshop
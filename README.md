## AWS CloudFormation stack
    This project is an infrastucture as a code(IaaS) demo for 2 application servers placed in private 
    subnets accessed by NAT gateway through public subnets.
    
![Alt text](cloudformation1.jpeg?raw=true "cloudFormation")

# Dependencies
    AWS CLI account that have sufficient access to resources.

# To run this project
    aws cloudformation create-stack --stack-name {stack name} --template-body file://{file name}.yml --region={region} --parameters file://{parameters file}.json --capabilities CAPABILITY_NAMED_IAM

    you will need to create network stack then servers stack as they depend on each other
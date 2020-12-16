# deploy_web_app_cloudformation
creates the network and servers in AWS using cloudformation

![alt text](https://github.com/dockingtheclouds/deploy_web_app_cloudformation/blob/main/Web-App-Infrastructure.jpeg?raw=true)

# myIfra.yaml and myInfra-params.json
These files will create a VPC, Internet Gateway, 2 public subnets, 2 private subnets,
 2 NAT Gateways, 2 Elastic IPs, and the route tables. You can change the parameters 
 by changing the params.json file to fit your needs. 
 
# server-params.json and final-project.yaml
These files will create a launch configuration, auto scaling group, load balancer, 
target groups, listeners, an IAM role for the ec2 instances, and the security groups. 
You can change the parameters by changing the params.json file to fit your needs.

# create.sh and update.sh 
You can use these scripts to create and update your cloudformation stack by adding 
the stack name, the yaml file, and then the json file that goes with the yaml file

# Introduction to Amazon RDS
This YAML file is a cloudformation template that creates the environment needed for the A Cloud Guru course Introduction to Amazon RDS (https://learn.acloud.guru/course/aws-rds/dashboard)

The basis for the file was taken from https://docs.aws.amazon.com/codebuild/latest/userguide/cloudformation-vpc-template.html

# Description
This template deploys a VPC, with a pair of public and private subnets spread across two Availability Zones. It deploys an internet gateway, with a default route on the public subnets. It deploys a pair of NAT gateways (one in each AZ), and default routes for them in the private subnets. It deploys a pair of RDS DB Subnet Groups, one for the pair of public subnets and one for the pair of private subnets.
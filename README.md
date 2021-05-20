# Cloudformation-Templates

This templates creates the following AWS components :

1. VPC - Allows user to set CIDR range for the VPC.
2. Subnets - Create 2 Public and 3 Private subnets in selected availability zones. 
3. Internet Gateway - Create Internet gateway and attach it to the VPC.
4. Nat Gateway - Create Nat Gateway in public subnet and attach Elastic IP address to it.
5. Route Tables - Create separate route tables for public and private subnets, setup routes and attach respective subnets to it.
6. NACL - Create custom NACL with Inbound and Outbound rules and associate it with subnets.
7. IAM role for Cloud watch Logs - Created IAM role, policies for Cloud watch VPC Logs.
8. VPC Flow logs - Create VPC Flow logs.
9. VPC Endpoint - Create VPC Endpoint and attach  route in Route tables.
10 . KMS - Creates a customer managed key.

The above templates provides the following components as output:

1. VPC ID
2. All Subnets ID
3.  KMS ID

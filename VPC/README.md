This templates creates the following AWS components :

VPC - Allows user to set CIDR range for the VPC.
Subnets - Create 2 Public and 3 Private subnets in selected availability zones.
Internet Gateway - Create Internet gateway and attach it to the VPC.
Nat Gateway - Create Nat Gateway in public subnet and attach Elastic IP address to it.
Route Tables - Create separate route tables for public and private subnets, setup routes and attach respective subnets to it.
NACL - Create custom NACL with Inbound and Outbound rules and associate it with subnets.
IAM role for Cloud watch Logs - Created IAM role, policies for Cloud watch VPC Logs.
VPC Flow logs - Create VPC Flow logs.
VPC Endpoint - Create VPC Endpoint and attach route in Route tables. 10 . KMS - Creates a customer managed key.
The above templates provides the following components as output:

VPC ID
All Subnets ID
KMS ID

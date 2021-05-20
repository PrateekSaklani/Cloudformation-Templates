This templates creates the following AWS components :

1. Document DB - Document DB Cluster.
2. Instances - Creates 2 instances in the cluster 1 would be Primary as writer and 1 would be reader. 
2. Security Group - Creates Security Group which would be attached to the Database.
3. Subnet Group - Creates Subnet group for document db with user provided subnets and associate it with DB.
4. Parameter Group - Creates the paramete group and associate it with the Databases.
5. Username/Password - Allows to create username and password for the Database with allow parameters.
6. Instance - Allows to select the instance type within the specified values.

Once all the resources are created it provides the Database Cluster Endpoint, Readers Endpoint and Database Security Group ID as output.
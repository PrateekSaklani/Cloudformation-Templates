This templates creates the following AWS components :

1. MSSQL - MSSQL Single Instance Database.
2. Security Group - Create a Security Group which would be attached to the Database.
3. Subnet Group - Create a Subnet group with user provided subnets and associate it with DB.
4. Parameter Group - Create the paramete group and associate it with the Databases.
5. Username/Password - Allows to create username and password for the Database with allow parameters.
6. Instance - Allows to select the instance type within the specified values.

Once all the resources are created it provides the Database Endpoint and Database Security Group ID as output.
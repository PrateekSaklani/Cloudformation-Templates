This templates creates the following AWS components :

1. ElasticCache - Redis instance with active and standby node.
2. Security Group - Creates Security Group which would be attached to the Redis.
3. Subnet Group - Creates Subnet group with user provided subnets and associate it with Redis.
4. Instance - Allows to select the instance type within the specified values.

Once all the resources are created it provides the Redis Endpoint.
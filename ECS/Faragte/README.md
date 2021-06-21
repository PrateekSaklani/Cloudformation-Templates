# Cloudformation-Templates

This templates creates the following AWS components :

1. TaskDefinition :
a. Register the task definitions for the container.
b. Creats an envoy proxy contianer for App mesh Routing purpose.
c. Push the container logs to the specified log group.
d. Picks up the other backend services like DB, Redis etc, connection string through Secret Manager using the environment value declare in the definition.

2. Servcies:
a. Creates the service for the container.
b. Creates the container in the specified subnets.
c. Map the containers to Load Balancer.
d. Setup the container with auto scaling capacity.
e. Creates the Cloud Watch alarm to scale the container according avg CPU value.
f. Creates the service discovery dns name which would be auto registered to Route53 and through App mesh other services would be able to commuincate with one another. 


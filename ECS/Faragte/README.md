# Cloudformation-Templates

This templates creates the following AWS components :

To prepare your application to run on Amazon ECS, you must create a task definition.
The task definition can be thought of as a blueprint for your application. It specifies various parameters for your application. For example, these parameters can be used to indicate which containers should be used, which ports should be opened for your application, and what data volumes should be used with the containers in the task.

An Amazon ECS service allows you to run and maintain a specified number of instances of a task definition simultaneously in an Amazon ECS cluster. If any of your tasks should fail or stop for any reason, the Amazon ECS service scheduler launches another instance of your task definition to replace it in order to maintain the desired number of tasks in the service.

1. TaskDefinition :
a. Register the task definitions for the container which includes the configuration of the container.
b. Creats an envoy proxy container for App mesh Routing purpose.
c. Push the container logs to the specified log group.
d. Picks up the other backend services like DB, Redis etc, connection string through Secret Manager using the environment value declared in the definition.

2. Service:
a. Creates the service for the container.
b. Creates the container in the specified subnets.
c. Map the containers to Load Balancer.
d. Setup the container with auto scaling capacity.
e. Creates the Cloud Watch alarm to scale the container according avg CPU threshold value.
f. Creates the service discovery dns name which would be auto registered to Route53 and through App mesh other services would be able to commuincate with one another. 


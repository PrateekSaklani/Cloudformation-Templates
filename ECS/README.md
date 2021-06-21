# Cloudformation-Templates

Amazon Elastic Container Service (Amazon ECS) is a fully managed container orchestration service that helps you easily deploy, manage, and scale containerized applications. It deeply integrates with the rest of the AWS platform to provide a secure and easy-to-use solution for running container workloads in the cloud and your infrastructure.

Over here we would using AWS Fargate to deploy our containers.

AWS Fargate is a serverless compute engine for containers that works with both Amazon Elastic Container Service (ECS) and Amazon Elastic Kubernetes Service (EKS). Fargate makes it easy for you to focus on building your applications. Fargate removes the need to provision and manage servers, lets you specify and pay for resources per application, and improves security through application isolation by design.

To deploy and run container in Fargate you require Cluster, Taskdefinition and Service.

Here are the Cloud Formation templates to register the Taskdifinition and create Service for the container.






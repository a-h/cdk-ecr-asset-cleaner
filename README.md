# cdk-ecr-asset-cleaner

A script that cleans out unused CDK Docker / ECR assets.

* Lists all of the containers in ECR.
* Searches through the ECS tasks and Lambda functions and find all the containers that were currently in use.
* * Prints out which ECS services and Lambda functions are using which containers in ECR.
* Does a diff between the in-use and not in-use containers.
* Prints out a list of all of the unused containers.
* Optionally deletes all the unused containers.

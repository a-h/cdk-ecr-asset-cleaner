# cdk-ecr-asset-cleaner

A script that cleans out unused CDK Docker / ECR assets.

* Searches through the ECS tasks and find all the containers that were currently in use.
* Lists all of the containers in ECR.
* Does a diff between the in-use and not in-use containers.
* Prints out which ECS services are using which containers in ECR.
* Prints out a list of all of the unused containers.
* Optionally deletes all the unused containers.

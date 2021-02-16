# udacity-devops-capstone
Capstone project for udacity devops class

# Folder Structure

The folder `cluster` contains CloudFormation script, `eks.yml`, 
to create a Kubernetes cluster named `EKS-udacity-capstone-cluster` using CloudFormation. Additional to the `eks.yml`, 
the file `aws-auth-configmap.yaml` to create a role and user for the managing the EKS cluster.

The folder `deploypment` defines the deployment to pull the Docker image from Docker Hub and deploy to a service `backend-master`.

# The Microservice

The microservice used in the deployment is hosted at the folder [`project-ml-microservice-kubernetes`](https://github.com/hungtruongquoc/DevOps_Microservices/tree/master/project-ml-microservice-kubernetes) of [this repository](https://github.com/hungtruongquoc/DevOps_Microservices/blob/master/.circleci/config.yml).

# The CI/CD Script

[The CI/CD script](https://github.com/hungtruongquoc/DevOps_Microservices/blob/master/.circleci/config.yml) is hosted in 
the [root folder](https://github.com/hungtruongquoc/DevOps_Microservices) of the repository of the microservice.

# The CI/CD Result

Screenshots of the CI/CD process are stored in `screenshots` folder. The result of each step are marked with sequential 
index from `1` to `6`. There are also 2 screenshots showing the CloudFormation stack of the Kubernetes cluster and node group.

# Notes

eksctl needs following environment variables:
```
AWS_DEFAULT_REGION
AWS_PROFILE
```

# RepoDeployer
Scalable tool built to deploy static websites.

[**Demo**](https://www.loom.com/share/92fbeccf53bf441488e710179a2c0e31?sid=4737d68b-dafc-4d13-bfc8-4dc13e9fd18c)

### Project Overview

- This project automates the deployment process by spinning up a Docker container that builds the code and pushes it to an S3 bucket.
- The Docker image used for this process is stored in the Elastic Container Registry (ECR).
- A cluster in the Elastic Container Service (ECS) accesses the Docker image from the ECR.
- The deployed code is accessed through a reverse proxy, which streams the data from the S3 bucket to the client.
- Logs generated during the deployment process are extracted from the container using a Redis pub/sub service.

### Technologies Used

- Docker 
- Node JS
- Elastic Container Registry (ECR)
- Elastic Container Service (ECS)
- Amazon S3 
- Redis
- Next JS/Typescript

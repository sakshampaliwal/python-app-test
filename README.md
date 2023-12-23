# Streamlining Code Releases with a CI/CD Pipeline on AWS

## Overview

This project demonstrates the implementation of a CI/CD pipeline using AWS services to automate the deployment of code changes, ensuring rapid and reliable application updates. The pipeline is triggered upon commits to a GitHub repository and leverages CodePipeline for orchestration, CodeBuild for building, and CodeDeploy for deployment.


## Technologies Used

- AWS CodePipeline
- AWS CodeBuild
- AWS CodeDeploy
- AWS Parameter Store
- Docker
- GitHub

## Setup and Configuration

### Prerequisites

- An AWS account with appropriate permissions
- A GitHub repository with your application code
- Configured CodeBuild and CodeDeploy services

### Pipeline Creation
Create an AWS CodePipeline
- Add a source stage linked to your GitHub repository
- Use Dockerfile to create a Docker image
- Use builspec.yml file for CodeBuild configuration
- Use appspec.yml file for CodeDeploy configuration
- Sensitive information such as passwords, tokens, or other crucial data should be securely stored. Utilize AWS Parameter Store for this
- Configure necessary permissions and settings
## Usage

1. Commit code changes to your GitHub repository.
2. The pipeline will automatically initiate the build and deployment process.
3. Monitor the pipeline's progress in the AWS CodePipeline console.

## Contributing

1. Fork this repository.
2. Create a branch for your changes.
3. Commit your changes and push to your branch.
4. Create a pull request.

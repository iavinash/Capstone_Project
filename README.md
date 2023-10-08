[![CircleCI](https://dl.circleci.com/status-badge/img/gh/iavinash/Capstone_Project/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/iavinash/Capstone_Project/tree/main)
# Capstone Project
The final project of the Cloud DevOps Udacity Nanodegree.

This repository contains the code and configuration for my Capstone project as part of the Udacity Cloud DevOps Nanodegree program.

## Project Overview

The Capstone project demonstrates my expertise in various DevOps and cloud technologies, including:

- AWS (Amazon Web Services): Utilizing AWS services to build and deploy cloud-based applications.
- CircleCI: Implementing continuous integration and continuous deployment pipelines for automated testing and deployment.
- Docker: Containerizing applications for consistency and portability.
- Kubernetes: Orchestrating containerized applications to scale and manage them efficiently.

## Project Structure

The repository is organized as follows:

- `app.py`: Contains the application code.
- `circleci/`: Contains CircleCI configuration files for automated builds and deployments.
- `ansible/`: Contains Ansible playbooks for configuring and deploying applications on Kubernetes clusters.
- `README.md`: The documentation you are currently reading.

## Deployment Process

1. CircleCI Pipeline:
    - Commits to this repository trigger CircleCI workflows.
    - The CI/CD pipeline consists of building, testing, and deploying the application.
    - Successful builds result in Docker images pushed to an ECR (Elastic Container Registry) repository.

2. Kubernetes Deployment:
    - Ansible playbooks are used to configure and deploy the application on Kubernetes clusters.
    - Blue-Green deployment strategy is employed to minimize downtime and risk during updates.


## Learnings

This Capstone project has been a valuable learning experience, allowing me to gain hands-on experience in cloud-based DevOps practices and technologies. I've learned to:

- Effectively use AWS services for cloud computing.
- Implement CI/CD pipelines with CircleCI.
- Containerize applications with Docker for consistent deployment.
- Manage container orchestration with Kubernetes.

## Note
To streamline the project setup process, please be aware that creating the `Amazon Elastic Container Registry` (ECR) and `Amazon Elastic Kubernetes` Service (EKS) cluster are separate steps that should be completed independently. 
We recommend using `eksctl` to create these resources, as it can help expedite the process. This separation is advised because CircleCI provisioning for these resources may take a longer duration.

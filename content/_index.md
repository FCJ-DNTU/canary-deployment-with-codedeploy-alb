+++
title = "Canary Deployment with CodeDeploy and Application Load Balancer"
date = 2025
weight = 1
chapter = false
+++

# Canary Deployment with CodeDeploy and Application Load Balancer

### Overview

In this workshop, you will:

- Understand how **Canary Deployment** works and the benefits it brings in a production environment.

- Learn how to leverage AWS services like **ECS**, **CodeDeploy**, **ALB**, **CloudWatch**, **X-Ray**, and **CodePipeline** to implement a complete canary strategy.

- Set up an automated **CI/CD** process that supports **traffic shifting**, **monitoring**, **automatic rollback**, and **A/B testing**.

- Be able to **safely deploy new versions**, minimize risks, and optimize user experience.

- Master tools for **monitoring and analyzing post-deployment performance**, helping you continuously improve release quality.

![AWS Architecture](/images/architecture.png)

### Objectives

- Clearly understand the concept and benefits of Canary Deployment.

- Grasp a real-world deployment architecture on AWS.

- Deploy a full Canary Deployment pipeline from source code to a production ECS service.

- Configure monitoring, alerting, automatic rollback, and basic A/B testing.

- Automate the entire CI/CD workflow with smart rollback capabilities.

### Prerequisites

**Required knowledge:**

- Basic knowledge of AWS (ECS, IAM, VPC, ALB).

- CI/CD concepts and Git workflow.

- Docker.

**Resources needed:**

- An AWS account.

- A sample code repository.

- A ready-to-use Docker image or knowledge of how to build one.

### Contents

1. [Introduction](1-introduction/)
2. [Deployment Architecture](2-deployment-architecture/)
3. [Environment Setup](3-setup-environment/)
4. [Build the CI/CD Pipeline](4-build-cicd-pipeline/)
5. [Monitoring & Automatic Rollback](5-monitoring-rollback/)
6. [A/B Testing with ALB Listener](6-ab-testing-alb/)
7. [Live Demo](7-demo/)

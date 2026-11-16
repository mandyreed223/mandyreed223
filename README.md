# Hi, I'm Mandy Reed 👋

**Enterprise IT professional | Aspiring AWS Cloud Engineer & DevOps Engineer**

I bring **18 years of hands-on IT support experience** in enterprise environments to my work in cloud engineering. I'm building practical skills through independent AWS and DevOps projects, with an emphasis on **infrastructure, automation, reliability, and troubleshooting**.

My favorite part isn't just getting something to deploy. It's understanding how the pieces connect, deliberately testing what happens when they fail, and documenting how I fixed them. ☁️🛠️

> **Build it. Break it responsibly. Troubleshoot it. Validate recovery. Document it.** 💚

## 🌐 Explore My Work

**[Live Cloud Engineering Portfolio](https://mandyreed.com)** · **[Technical Stories on Medium](https://medium.com/@mandymreed)** · **[Connect on LinkedIn](https://www.linkedin.com/in/mandymreed/)**

My portfolio is itself a cloud project: a **private Amazon S3 origin behind CloudFront OAC**, HTTPS with ACM and Route 53, **GitHub Actions deployments using OIDC and an IAM role**, and a **Terraform-managed visitor counter** built with API Gateway, Lambda, and DynamoDB. Website changes deploy through GitHub Actions; visitor-counter infrastructure is currently managed with Terraform separately.

## ⭐ Featured Cloud & DevOps Projects

### 🏗️ [Highly Available 2-Tier AWS Architecture with Terraform](https://github.com/mandyreed223/terraform-ha-2tier-aws)

Designed a production-inspired AWS architecture across two Availability Zones with **private EC2 instances, an Application Load Balancer, Auto Scaling, Multi-AZ RDS MySQL, Secrets Manager, Systems Manager, and CloudWatch**. Deliberately terminated compute, verified Auto Scaling recovery, and confirmed database records persisted.

### ⚡ [Real-Time AWS Network Telemetry Pipeline](https://github.com/mandyreed223/aws-realtime-network-telemetry)

Built an event-driven pipeline with **Terraform, Kinesis Data Streams, Lambda, DynamoDB, SQS, CloudWatch, and SNS**. Tested malformed-record quarantine, failed-batch handling, partial-batch failures, and idempotent writes to understand how streaming systems recover when events don't go as planned.

📖 [Read the story: My Kitten Had Other Plans](https://medium.com/@mandymreed/%EF%B8%8F-i-built-a-real-time-aws-pipeline-my-kitten-had-other-plans-81ba484f1f1b)

### ☁️ [CloudFormation WordPress Automation](https://github.com/mandyreed223/aws-cloudformation-wordpress-automation)

Built a multi-tier WordPress environment with **AWS CloudFormation, an ALB, Auto Scaling, EFS, Multi-AZ RDS MariaDB, Secrets Manager, ACM, Route 53, and CloudWatch**. Validated manual capacity changes and failure/recovery behavior. EventBridge Scheduler schedules were defined but **left disabled by default**.

📖 [Read the story: Four Days of CloudFormation Chaos](https://medium.com/@mandymreed/%EF%B8%8F-i-turned-a-simple-aws-assignment-into-four-days-of-cloudformation-chaos-b3d389e7bff5)

### 🚀 [Jenkins CI/CD Pipeline to AWS ECS Fargate](https://github.com/mandyreed223/jenkins-cicd-aws-pipeline)

Built a pipeline from **GitHub → Jenkins → Docker → Amazon ECR → ECS/Fargate**, with a quality gate that stopped a deliberately broken release before deployment. Validated a successful release and ECS task recovery.

### 🏗️ [Terraform Auto Scaling Architecture](https://github.com/mandyreed223/terraform-asg-deployment)

Provisioned AWS networking, private EC2 instances, an ALB, and an Auto Scaling Group using Terraform. Traced failed health checks to a whitespace error in EC2 User Data, corrected the Launch Template, and rolled out the fix with Instance Refresh.

### ☸️ [Amazon EKS Deployment](https://github.com/mandyreed223/amazon-eks-deployment)

Deployed a containerized application using **EKS, ECR, Kubernetes Deployments, Services, and Horizontal Pod Autoscaling**. Tested self-healing, rolling updates, and CPU-driven scaling.

**[Browse all projects and filter by Architecture, IaC, CI/CD, Containers, or Serverless →](https://mandyreed.com)**

## 🛠️ Technical Toolkit

| Area | Hands-on experience |
| --- | --- |
| **AWS architecture** | VPC, EC2, ALB, Auto Scaling, RDS, EFS, S3, CloudFront, Route 53, ACM, IAM, Systems Manager |
| **Infrastructure as Code** | Terraform, CloudFormation, resource references, remote state, infrastructure troubleshooting |
| **Serverless & events** | Lambda, API Gateway, DynamoDB, Kinesis, SQS, SNS, EventBridge Scheduler |
| **CI/CD & automation** | GitHub Actions, OIDC federation, Jenkins, Git, AWS CLI, Python, Linux |
| **Containers** | Docker, Docker Swarm, Kubernetes, Amazon EKS, ECR, ECS/Fargate |
| **Operations & reliability** | CloudWatch, alarms, health checks, failure testing, recovery validation, documentation |
| **Enterprise IT** | Microsoft 365, Active Directory, ServiceNow, incident management, user support |

## 🎯 Current Focus

I'm preparing for the **AWS Certified Solutions Architect – Associate** exam while continuing to build and troubleshoot AWS projects. My current learning priorities are **AWS architecture, reliability, monitoring, infrastructure automation, and operational troubleshooting**. I'll explore additional cloud platforms after the exam.

## ✍️ Why I Document the Chaos

I write about what I built, what broke, how I investigated it, and what I learned. My projects are intentionally hands-on: a green deployment is the beginning of validation, not the end.

📖 **[Read my technical project stories on Medium](https://medium.com/@mandymreed)**

## 📫 Connect

🌐 [Portfolio](https://mandyreed.com) · 💼 [LinkedIn](https://www.linkedin.com/in/mandymreed/) · ✍️ [Medium](https://medium.com/@mandymreed) 

---

☁️ **Build it. Troubleshoot it. Understand it. Then build something harder.** 🚀

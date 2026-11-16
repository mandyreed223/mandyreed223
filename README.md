# Hi, I'm Mandy Reed 👋

**Enterprise IT Professional | Aspiring AWS Cloud Engineer & DevOps Engineer**

I bring **18 years of hands-on IT experience** supporting users and business-critical technology in enterprise environments, and I'm building on that foundation through independent Cloud Engineering and DevOps projects.

My hands-on experience includes AWS, Terraform, CloudFormation, Infrastructure as Code, Linux, Docker, Kubernetes, Amazon EKS, CI/CD pipelines, automation, monitoring, and highly available cloud architectures.

I enjoy understanding how systems connect, troubleshooting what happens when they don't, and documenting what I learn along the way.

My favorite part isn't just getting something deployed. It's testing what happens when things break and figuring out how to make them work again. ☁️🛠️

> **Build it. Break it responsibly. Troubleshoot it. Validate recovery. Document it.** 💚

---

## 🌐 Explore My Work

🚀 **[Live Cloud Engineering Portfolio](https://mandyreed.com)**

📖 **[Technical Stories on Medium](https://medium.com/@mandymreed)**

💼 **[Connect on LinkedIn](https://www.linkedin.com/in/mandymreed/)**

My portfolio is also an active AWS project.

It uses Amazon S3, CloudFront Origin Access Control (OAC), Route 53, AWS Certificate Manager, and HTTPS for secure content delivery.

GitHub Actions automatically deploys website changes using OIDC federation and a least-privilege IAM role.

I also built a **Terraform-managed serverless visitor counter** using API Gateway, Lambda, and DynamoDB.

The website deployment is automated through GitHub Actions, while the visitor-counter infrastructure is currently managed separately through Terraform.

---

## ⭐ Featured Cloud & DevOps Projects

### 🏗️ [Highly Available 2-Tier AWS Architecture with Terraform](https://github.com/mandyreed223/terraform-ha-2tier-aws)

Designed a production-inspired AWS architecture across two Availability Zones with **private EC2 instances, an Application Load Balancer, Auto Scaling, Multi-AZ RDS MySQL, Secrets Manager, Systems Manager, and CloudWatch**.

Deliberately terminated compute, verified Auto Scaling recovery, monitored application health, and confirmed database records persisted after instance replacement.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/i-built-a-highly-available-aws-architecture-then-i-started-killing-ec2-instances-6f6996657256)

### ⚡ [Real-Time AWS Network Telemetry Pipeline](https://github.com/mandyreed223/aws-realtime-network-telemetry)

Built an event-driven pipeline with **Terraform, Kinesis Data Streams, Lambda, DynamoDB, SQS, CloudWatch, and SNS**.

Tested malformed-record quarantine, failed-batch handling, partial-batch failures, and idempotent writes to understand how streaming systems recover when events don't go as planned.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/%EF%B8%8F-i-built-a-real-time-aws-pipeline-my-kitten-had-other-plans-81ba484f1f1b)

### ☁️ [CloudFormation WordPress Automation](https://github.com/mandyreed223/aws-cloudformation-wordpress-automation)

Built a multi-tier WordPress environment using **AWS CloudFormation, an Application Load Balancer, Auto Scaling, Amazon EFS, Multi-AZ RDS MariaDB, Secrets Manager, ACM, Route 53, and CloudWatch**.

Validated manual capacity changes and failure/recovery behavior.

EventBridge Scheduler schedules were defined but **left disabled by default**.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/%EF%B8%8F-i-turned-a-simple-aws-assignment-into-four-days-of-cloudformation-chaos-b3d389e7bff5)

### 🚀 [Jenkins CI/CD Pipeline to AWS ECS Fargate](https://github.com/mandyreed223/jenkins-cicd-aws-pipeline)

Built an end-to-end deployment pipeline connecting **GitHub, Jenkins, Docker, Amazon ECR, Amazon ECS, and AWS Fargate**.

Implemented an application quality gate that successfully blocked a deliberately broken release before it could reach production.

Validated successful deployments and ECS task recovery.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/i-built-a-ci-cd-pipeline-then-i-broke-the-pipeline-2397aae6bc7b)

### 🏗️ [Terraform Auto Scaling Architecture](https://github.com/mandyreed223/terraform-asg-deployment)

Provisioned AWS networking, private EC2 instances, an Application Load Balancer, and an Auto Scaling Group using Terraform.

Traced failed Target Group health checks to a whitespace error in EC2 User Data, corrected the Launch Template, and rolled out the fix using EC2 Instance Refresh.

Tested Auto Scaling recovery by deliberately terminating an instance.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/%EF%B8%8F-i-built-an-auto-scaling-architecture-with-terraform-then-one-tiny-space-broke-everything-c1f29147dcd5)

### ☸️ [Amazon EKS Deployment](https://github.com/mandyreed223/amazon-eks-deployment)

Deployed and operated a containerized application using **Amazon EKS, Amazon ECR, Kubernetes Deployments, Services, and Horizontal Pod Autoscaling**.

Tested Kubernetes self-healing by deliberately deleting Pods, performed rolling application updates, and validated CPU-driven scaling.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/i-put-kubernetes-on-aws-then-i-started-deleting-pods-%EF%B8%8F-6b5d9898773a)

### 🔎 Explore More Projects

These are just a few of my hands-on projects.

My portfolio also includes Docker Swarm, Kubernetes troubleshooting, serverless AWS applications, Jenkins infrastructure, GitHub Actions automation, and additional cloud engineering labs.

**[Browse All Projects by Architecture, IaC, CI/CD, Containers, or Serverless →](https://mandyreed.com)**

---

## 🛠️ Technical Toolkit

| Area | Hands-On Experience |
|---|---|
| **AWS Architecture** | VPC, EC2, ALB, Auto Scaling, RDS, EFS, S3, CloudFront, Route 53, ACM, IAM, Systems Manager |
| **Infrastructure as Code** | Terraform, CloudFormation, resource references, remote state, infrastructure troubleshooting |
| **Serverless & Event-Driven AWS** | Lambda, API Gateway, DynamoDB, Kinesis, SQS, SNS, EventBridge Scheduler |
| **CI/CD & Automation** | GitHub Actions, OIDC federation, Jenkins, Git, AWS CLI, Python, Linux |
| **Containers & Orchestration** | Docker, Docker Swarm, Kubernetes, Amazon EKS, ECR, ECS/Fargate |
| **Monitoring & Reliability** | CloudWatch, alarms, health checks, failure testing, recovery validation |
| **Enterprise IT** | Microsoft 365, Active Directory, ServiceNow, incident management, technical troubleshooting |

---

## 🎯 Current Focus

I'm currently preparing for the **AWS Certified Solutions Architect – Associate (SAA-C03)** certification.

While studying, I'm continuing to strengthen my AWS knowledge through hands-on projects involving:

- AWS architecture and networking
- Infrastructure as Code with Terraform and CloudFormation
- Event-driven and serverless architectures
- Monitoring, reliability, and recovery testing
- CI/CD and deployment automation
- Cloud security and operational troubleshooting

My immediate focus is AWS. I plan to explore additional cloud platforms after completing my certification.

---

## 🧠 My Engineering Approach

I believe a successful deployment is only the beginning.

An EC2 instance can show `running` while the application is broken.

A Kubernetes Pod can show `Running` while the service is unreachable.

Terraform can successfully provision infrastructure while a bootstrap script silently fails.

And a CI/CD pipeline should stop a broken release before it reaches production.

That's why I focus on understanding the entire system rather than just individual services.

**Build → Test → Break → Troubleshoot → Validate → Document**

---

## ✍️ Documenting the Journey

I write about my cloud engineering projects on Medium, including what I built, what went wrong, how I approached troubleshooting, and what I learned.

My articles aren't just deployment tutorials. They're stories about the engineering process, including the occasional four-day troubleshooting adventure or unexpected kitten interruption. 😂🐾

📖 **[Read My Cloud & DevOps Stories on Medium](https://medium.com/@mandymreed)**

---

## 📫 Connect With Me

🌐 **Portfolio:** [mandyreed.com](https://mandyreed.com)

💼 **LinkedIn:** [linkedin.com/in/mandymreed](https://www.linkedin.com/in/mandymreed/)

✍️ **Medium:** [medium.com/@mandymreed](https://medium.com/@mandymreed)

---

☁️ **Build it. Troubleshoot it. Understand it. Then build something harder.** 🚀

# Hi, I'm Mandy Reed 👋

I'm a Service Desk Analyst with 18 years of IT experience supporting users in enterprise environments, and I'm expanding that experience into Cloud Engineering and DevOps.

Through hands-on projects and continuous learning, I'm building practical experience with AWS, Terraform, Infrastructure as Code, highly available cloud architectures, EC2 Auto Scaling, Application Load Balancing, Amazon EKS, Amazon ECR, Linux, Docker, Kubernetes, container orchestration, autoscaling, monitoring, CI/CD pipelines, cloud automation, and cloud platform operations.

I enjoy understanding how the pieces connect, troubleshooting what happens when they don't, and documenting what I learn along the way. ☁️🛠️

## 🌐 Portfolio

🚀 **Cloud Engineering Portfolio**

🌐 [mandyreed.com](https://mandyreed.com)

My personal cloud engineering portfolio is hosted on AWS using Amazon S3, CloudFront, Route 53, and AWS Certificate Manager with a custom domain and HTTPS.

## 🎯 Current Focus

* Microsoft Azure
* Site Reliability Engineering (SRE)
* Monitoring and Alerting
* Cloud Security
* Kubernetes Observability
* Deployment Automation
* Deeper Terraform Automation
* Expanding AWS, Terraform, and Kubernetes skills through increasingly production-inspired architectures and operational troubleshooting

## ☁️ Cloud & DevOps Skills

### AWS

* EC2
* EC2 Auto Scaling
* Launch Templates
* Application Load Balancer
* Target Groups
* AWS Systems Manager
* S3
* EFS
* Amazon EKS
* Amazon ECR
* Amazon VPC
* Public and Private Subnets
* NAT Gateway
* Internet Gateway
* Route Tables
* Security Groups
* Elastic Load Balancing
* Lambda
* CloudFront
* Route 53
* AWS Certificate Manager
* IAM
* CloudWatch
* DynamoDB
* API Gateway
* Amazon Polly
* Amazon Rekognition
* Amazon Transcribe
* Amazon Translate
* Amazon Bedrock

### DevOps & Automation

* Terraform
* Infrastructure as Code (IaC)
* Terraform Resource References
* Terraform Remote State
* S3 State Versioning
* Terraform State Locking
* EC2 Instance Refresh
* Git
* GitHub
* GitHub Actions
* CI/CD Pipelines
* Docker
* Dockerfiles
* Docker Compose
* Docker Swarm
* Docker Stack
* Docker Secrets
* Docker Networking
* Docker Image Versioning
* Container Troubleshooting
* Overlay Networking
* Persistent Volumes
* Jenkins
* AWS CLI

### Kubernetes & Container Orchestration

* Kubernetes
* Amazon EKS
* MicroK8s
* kubectl
* eksctl
* Pods
* Deployments
* ReplicaSets
* Services
* ClusterIP
* LoadBalancer Services
* Labels and Selectors
* EndpointSlices
* Declarative YAML
* Scaling
* Horizontal Pod Autoscaling (HPA)
* Metrics Server
* Resource Requests and Limits
* Desired-State Reconciliation
* Self-Healing Workloads
* Rolling Updates
* Managed Node Groups
* Multi-Tier Applications
* Application-to-Database Communication
* Persistent Application Data
* Kubernetes Networking
* Kubernetes Troubleshooting

### Applications & Data

* Apache HTTP Server
* nginx
* WordPress
* MySQL
* Shared File Storage
* NFS
* Persistent Application Data

### Operating Systems

* Linux
* Windows

### IT Operations

* Active Directory
* Microsoft 365
* ServiceNow
* Incident Management
* User Access Management

## 🚀 Featured Projects

### 🏗️ Terraform Auto Scaling Architecture on AWS

🔗 [View Repository](https://github.com/mandyreed223/terraform-asg-deployment)

**I built an Auto Scaling architecture with Terraform. Then one tiny space broke everything. 😅**

Built a highly available AWS web architecture with Terraform using a custom VPC, public and private subnets across multiple Availability Zones, an internet-facing Application Load Balancer, and an Auto Scaling Group running EC2 instances in private subnets.

Used a Launch Template to define EC2 configuration, AWS Systems Manager Session Manager for secure administration without inbound SSH, NAT for outbound connectivity, and Amazon S3 remote Terraform state with versioning and state locking.

Validated load balancing and self-healing by deliberately terminating a healthy EC2 instance and watching the Auto Scaling Group restore desired capacity.

During an application update, troubleshot failed Target Group health checks through the complete request path and discovered that a single leading space before the `#!/bin/bash` shebang prevented EC2 User Data from running correctly. Corrected the bootstrap script, created a new Launch Template version, and used EC2 Instance Refresh to roll the fixed configuration across the fleet.

The project strengthened my understanding of Terraform resource linkage by following values between resources: subnet IDs feed the load balancer and Auto Scaling Group, the Target Group connects the ALB to the fleet, the Launch Template defines the EC2 instances, and the Auto Scaling Group turns those definitions into running infrastructure.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/%EF%B8%8F-i-built-an-auto-scaling-architecture-with-terraform-then-one-tiny-space-broke-everything-c1f29147dcd5)

### ☁️☸️ Amazon EKS Deployment

🔗 [View Repository](https://github.com/mandyreed223/amazon-eks-deployment)

**I put Kubernetes on AWS. Then I started deleting Pods. ☸️😈**

Moved my Kubernetes learning from a local environment into AWS by building, deploying, scaling, monitoring, updating, and troubleshooting a containerized application on Amazon Elastic Kubernetes Service (EKS).

Built a managed EKS cluster with private EC2 worker nodes across two Availability Zones, pushed versioned Docker images to Amazon ECR, and exposed the application through a Kubernetes LoadBalancer Service.

Added resource requests and limits, Metrics Server, and Horizontal Pod Autoscaling, then generated CPU load to watch the application automatically scale from three Pods to four and return to three as demand decreased.

Tested Kubernetes self-healing by deliberately deleting Pods, performed a rolling application update using a new ECR image version, and enabled EKS API and audit logging in Amazon CloudWatch.

The project helped connect the complete path from local application code to Docker, Amazon ECR, Kubernetes workloads, AWS load balancing, autoscaling, compute, networking, and monitoring.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/i-put-kubernetes-on-aws-then-i-started-deleting-pods-%EF%B8%8F-6b5d9898773a)

### ☸️ WordPress + MySQL Multi-Tier Application on Kubernetes

🔗 [View Repository](https://github.com/mandyreed223/kubernetes-multitier-application)

Built a multi-tier WordPress and MySQL application on Kubernetes, moving beyond individual Kubernetes resources to explore how application and database workloads communicate as part of a larger system.

Worked with Deployments, Services, labels and selectors, persistent application data, Kubernetes networking, and application-to-database communication while troubleshooting the complete path between WordPress and MySQL.

The project reinforced an important lesson: a Pod showing `Running` does not automatically mean the application is healthy. Troubleshooting required following the relationships between workloads, Services, configuration, storage, networking, database connectivity, and the application itself.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/i-put-wordpress-and-mysql-on-kubernetes-then-mysql-fought-back-%EF%B8%8F-05a6370e0926)

### ☸️ Kubernetes Fundamentals

🔗 [View Repository](https://github.com/mandyreed223/kubernetes-fundamentals)

Built my first hands-on Kubernetes application using MicroK8s on Ubuntu in WSL2, progressing from a standalone nginx Pod to a declaratively managed application using Deployments, ReplicaSets, multiple Pods, and a ClusterIP Service.

Practiced scaling, labels and selectors, EndpointSlices, rolling updates, and desired-state reconciliation while intentionally deleting a Pod to observe Kubernetes self-healing.

Finished by moving the application into reusable YAML and troubleshooting an immutable Deployment selector while rebuilding and validating the environment declaratively.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/kubernetes-said-desired-state-i-said-prove-it-%EF%B8%8F-e8fbe1469ec3)

### 🐳 WordPress + MySQL Docker Swarm on AWS

🔗 [View Repository](https://github.com/mandyreed223/wordpress-docker-swarm-aws)

Built a multi-service WordPress and MySQL application across a three-node Docker Swarm running on AWS EC2.

Used Docker Stack, overlay networking, Docker Secrets, and Amazon EFS shared storage to explore multi-service orchestration, persistent application data, service communication, and resiliency.

Tested recovery by removing a worker node and observing Swarm reschedule workloads, while troubleshooting Linux, Docker, networking, SSH, storage, and AWS infrastructure along the way.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/i-put-wordpress-on-docker-swarm-then-things-got-real-438cbb166861)

### 🐳 Docker Swarm on AWS

🔗 [View Repository](https://github.com/mandyreed223/docker-swarm-aws-lab)

Built a three-node Docker Swarm across AWS EC2 instances to practice multi-node container orchestration, replicated and global services, scaling, self-healing, Docker Stack, overlay networking, and routing mesh.

Tested cluster resiliency by intentionally removing containers and draining a worker node to validate desired-state recovery, task rescheduling, and traffic routing across the Swarm.

📖 [Read the Project Story on Medium](https://medium.com/@mandymreed/i-built-a-docker-swarm-then-i-started-killing-containers-14bfd9fb54ae)

### 🏗️ Jenkins on AWS with Terraform

🔗 [View Repository](https://github.com/mandyreed223/terraform-jenkins-aws)

Deployed Jenkins on AWS using Terraform, progressing from a manual proof of concept to reusable Infrastructure as Code.

Provisioned EC2, Security Groups, and private S3 artifact storage, automated Jenkins installation with User Data, and implemented an IAM Role and Instance Profile with least-privilege S3 permissions.

Validated temporary AWS credentials and tested artifact upload and download before safely destroying the Terraform-managed infrastructure.

### 🐳 Docker + Jenkins Lab

🔗 [View Repository](https://github.com/mandyreed223/docker-jenkins-lab)

Built and managed Jenkins in Docker while exploring container lifecycle, persistent storage, Docker Compose, and custom image creation.

Tested data persistence by intentionally removing and recreating containers, then built a custom Jenkins image using a Dockerfile.

### 🐳 Docker + Apache Web App Rebuild

🔗 [View Repository](https://github.com/mandyreed223/docker-apache-webapp)

Revisited and rebuilt one of my earliest Docker projects after gaining more hands-on experience with containers, networking, and troubleshooting.

Used Dockerfiles and reusable images while practicing image versioning, layer caching, port mapping, Docker networking, container inspection, lifecycle management, and application validation.

The rebuild turned an early Docker exercise into an opportunity to compare how I approached the same technology after gaining more hands-on experience.

**Same project. Different engineer. 🐳**

📖 [Read the Updated Project Story on Medium](https://medium.com/@mandymreed/it-worked-on-my-machine-until-it-didnt-3d2df233c995)

### 🌐 Cloud Engineering Portfolio

🔗 [View Repository](https://github.com/mandyreed223/cloud-engineer-portfolio)

Built and deployed a personal cloud portfolio using HTML, CSS, Amazon S3, CloudFront, Route 53, and AWS Certificate Manager with a custom domain and HTTPS.

🌐 [View Live Portfolio](https://mandyreed.com)

### 🤖 Prompt Deployment Pipeline

🔗 [View Repository](https://github.com/mandyreed223/prompt-deployment-pipeline)

Built a CI/CD-style workflow using GitHub, Amazon S3, and Amazon Bedrock.

### 🌎 Multilingual Audio Pipeline

🔗 [View Repository](https://github.com/mandyreed223/multilingual-audio-pipeline)

Created an AWS workflow using Amazon Transcribe, Translate, Polly, Lambda, S3, and CloudWatch logging.

### 🖼️ Rekognition Image Labeling Pipeline

🔗 [View Repository](https://github.com/mandyreed223/rekognition-image-labeling-pipeline)

Built an image-processing workflow using Amazon Rekognition, Lambda, DynamoDB, GitHub Actions, and CloudWatch.

### 🔊 Polly Text-to-Speech Pipeline

🔗 [View Repository](https://github.com/mandyreed223/polly_text_to_speech_pipeline)

Created a serverless text-to-speech solution using Amazon Polly, Lambda, API Gateway, S3, and CloudWatch.

### ✅ Required Files Checker

🔗 [View Repository](https://github.com/mandyreed223/file_checker_project)

Built a GitHub Actions workflow that validates required repository files and sends logs to Amazon CloudWatch.

## ✍️ Project Stories & Technical Writing

📖 [Read my technical writing on Medium](https://medium.com/@mandymreed)

I document hands-on projects, troubleshooting experiences, lessons learned, and the occasional **“why is THAT happening?”** moment. 😅

My articles focus not only on what I built, but also on what went wrong, how I approached troubleshooting, and what I learned from the experience.

Recent stories include:

* 🏗️ **I Built an Auto Scaling Architecture with Terraform. Then One Tiny Space Broke Everything. 😅**
* ☁️☸️ **I Put Kubernetes on AWS. Then I Started Deleting Pods. ☸️😈**
* ☸️ **I Put WordPress and MySQL on Kubernetes. Then MySQL Fought Back. ⚔️**
* ☸️ **Kubernetes Said Desired State. I Said Prove It.**
* 🐳 **I Put WordPress on Docker Swarm. Then Things Got Real.**
* 🐳 **I Built a Docker Swarm. Then I Started Killing Containers.**
* 🏗️ **Jenkins on AWS with Terraform**
* 🐳 **Docker + Jenkins**
* 🐳 **It Worked on My Machine... Until It Didn't: Revisited**
* 🌐 **Building My AWS Cloud Engineering Portfolio**

## 📫 Connect With Me

🌐 **Portfolio:** [mandyreed.com](https://mandyreed.com)

💼 **LinkedIn:** [linkedin.com/in/mandymreed](https://www.linkedin.com/in/mandymreed/)

💻 **GitHub:** [github.com/mandyreed223](https://github.com/mandyreed223)

✍️ **Medium:** [medium.com/@mandymreed](https://medium.com/@mandymreed)

---

☁️ **Build it. Troubleshoot it. Understand it. Then build something harder.** 🚀

# 🚀 Serverless CI/CD Pipeline using AWS Lambda

A **fully serverless CI/CD pipeline** built on AWS that automatically deploys code from a **GitHub repository** to an **S3 static website**, all without EC2 or Jenkins.

This project demonstrates **event-driven DevOps automation** using AWS native services.

---
## 🛠️ **Architecture Workflow**

![](assets/very.png)

## 🧩 **Project Overview**

Whenever you push code to the GitHub repository:
1. **GitHub Webhook** triggers an **API Gateway endpoint**
2. **AWS Lambda** starts the **AWS CodePipeline**
3. **CodePipeline** uses **AWS CodeBuild** to build/test the application
4. Build artifacts are deployed to **Amazon S3**
5. **Amazon CloudFront** delivers the static site globally
6. **Amazon CloudWatch** monitors logs and events
7. **AWS IAM** manages access and permissions

---
## Tech stack
| Category       | Service                | Description                             |
| -------------- | ---------------------- | --------------------------------------- |
| Source Control | **GitHub**             | Stores source code & triggers webhook   |
| API Gateway    | **Amazon API Gateway** | Receives webhook event from GitHub      |
| Compute        | **AWS Lambda**         | Executes function to start CodePipeline |
| CI/CD          | **AWS CodePipeline**   | Orchestrates build & deployment         |
| Build          | **AWS CodeBuild**      | Compiles and tests code                 |
| Storage        | **Amazon S3**          | Hosts the static website                |
| Delivery       | **Amazon CloudFront**  | Delivers content globally               |
| Security       | **AWS IAM**            | Manages permissions and access          |

---
## 🧠 DevOps Concepts Demonstrated
- Serverless CI/CD automation

- Event-driven architecture

- GitHub webhook integration

- AWS-native CI/CD pipeline

- Infrastructure-as-Code mindset (manual setup, IaC optional)

- Cloud security & monitoring best practices
---




# Enterprise-Kubernetes-Platform-EKS-Landing-Zone-
A Fortune 500 company wants a reusable Kubernetes platform where developers only push code.  Everything else is automated.

GitHub

      │

GitHub Actions

      │

Terraform

      │

AWS

├── VPC
├── EKS
├── Managed Node Groups
├── IAM Roles
├── ECR
├── ALB Controller
├── Metrics Server
├── Cluster Autoscaler
├── Karpenter
├── EFS
├── EBS CSI
├── CloudWatch
└── Route53

Terraform provisions

* Enterprise VPC
* EKS Cluster
* Managed Node Groups
* IAM OIDC
* ECR
* Security Groups
* EFS
* KMS
* CloudWatch
* IAM Roles
* ALB Controller
* Cluster Autoscaler
* Karpenter
* ExternalDNS

Ansible configures

Provision a separate management EC2 server.

Install

* kubectl
* Helm
* AWS CLI
* eksctl
* ArgoCD CLI
* Prometheus CLI
* Grafana provisioning
* Terraform
* Docker

Then automatically

Deploy

* Prometheus
* Grafana
* Loki
* Tempo
* Alertmanager
* ArgoCD
* Cert Manager
* ExternalDNS
* NGINX Ingress
* Metrics Server

⸻

GitHub Actions

Pipeline 1
Terraform Validate

↓

Terraform Plan

↓

Approval

↓

Terraform Apply

↓

Run Ansible

↓

Verify Cluster

Pipeline 2

Application Deployment
Developer Push

↓

Build Docker Image

↓

Unit Tests

↓

Scan Image (Trivy)

↓

Push to ECR

↓

Update Helm Chart

↓

Deploy to EKS

↓

Smoke Test

↓

Slack Notification

Pipeline 3

Destroy Environment
Approval

↓

Terraform Destroy

↓

Cleanup

Bonus Enterprise Features

Add these to make your portfolio stand out:

* Multi-environment (Dev/QA/UAT/Prod)
* Terraform remote backend (S3 + DynamoDB)
* GitHub OIDC authentication (no AWS keys)
* Checkov security scans
* TFLint
* Trivy image scanning
* Dependabot
* Semantic versioning
* Reusable GitHub Actions workflows
* Terraform modules
* Dynamic Ansible inventory
* CloudWatch dashboards
* Cost estimation
* Automatic rollback
* Blue/Green deployment
* Canary deployment
* Slack or Microsoft Teams notifications

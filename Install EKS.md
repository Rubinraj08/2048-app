# ☁️ Amazon EKS Cluster on Fargate

This guide documents how to create and delete an Amazon EKS cluster that uses AWS Fargate as the compute engine.

---

## 🚀 1. Create EKS Cluster Using Fargate

Use the following command to create a new EKS cluster named `demo-cluster` with Fargate profiles automatically set up.

```cmd
eksctl create cluster --name demo-cluster --region us-east-1 --fargate

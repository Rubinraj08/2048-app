# 2048 App

This project deploys the classic 2048 game application on AWS using Kubernetes.  
It uses an Application Load Balancer to control traffic and provides access to the application through an Ingress and Ingress Controller.

---

## 🔧 Technologies Used

- **AWS**
- **Kubernetes**

---

## 🧰 AWS Services Used

- IAM User  
- IAM Policies  
- Elastic Compute Cloud (EC2)  
- Elastic Kubernetes Service (EKS)

---

## 🚀 Features

- ✅ Provided Application Load Balancer to control the number of requests to the application  
- ✅ Easily accessible for end users using Ingress and Ingress Controller

---

## 📦 Deploy the App

Apply the deployment, service, and ingress using:
kubectl apply -f 2048_full.yaml

🔐 Create IAM Policy
aws iam create-policy --policy-name AWSLoadBalancerControllerIAMPolicy --policy-document file://iam_policy.json

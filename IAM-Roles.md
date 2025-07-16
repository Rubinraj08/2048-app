# 🔐 Create IAM Role for AWS Load Balancer Controller

This step creates an IAM service account and attaches the required IAM policy for the AWS Load Balancer Controller in your EKS cluster.

---

## ✅ Command (for Windows CLI / PowerShell)

```cmd
eksctl create iamserviceaccount --cluster=demo-cluster-1 --namespace=kube-system --name=aws-load-balancer-controller --role-name AmazonEKSLoadBalancerControllerRole --attach-policy-arn=arn:aws:iam::<your_aws_id>:policy/AWSLoadBalancerControllerIAMPolicy –approve

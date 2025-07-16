# 🔐 Configure IAM OIDC Provider for Amazon EKS


```cmd
export cluster_name=demo-cluster
```

```cmd
oidc_id=$(aws eks describe-cluster --name $cluster_name --query "cluster.identity.oidc.issuer" --output text | cut -d '/' -f 5)
```
Check if there is an IAM OIDC provider configured already
---
If not, run the below command
```
eksctl utils associate-iam-oidc-provider --cluster $cluster_name --approve

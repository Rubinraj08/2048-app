# 🪟 Install AWS Load Balancer Controller on Amazon EKS (Windows CLI)
---

## 1️⃣ Add the Helm Repository

Open **Command Prompt** or **PowerShell**, then run:

```cmd
helm repo add eks https://aws.github.io/eks-charts

2️⃣ Install the Controller with Helm
helm install aws-load-balancer-controller eks/aws-load-balancer-controller -n kube-system --set clusterName=demo-cluster-1 --set serviceAccount.create=false --set serviceAccount.name=aws-load-balancer-controller --set region=us-east-1 --set vpcId=vpc-<your_vpc_id>

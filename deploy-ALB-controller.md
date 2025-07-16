1.Add helm repo
helm repo add eks https://aws.github.io/eks-charts

2.Install
helm install aws-load-balancer-controller eks/aws-load-balancer-controller -n kube-system --set clusterName=demo-cluster-1 --set serviceAccount.create=false --set serviceAccount.name=aws-load-balancer-controller --set region=us-east-1 --set vpcId=vpc-009efd5b48dab07ba

3.Verify that the deployments are running.
kubectl get deployment -n kube-system aws-load-balancer-controller

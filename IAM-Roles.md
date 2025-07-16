Create IAM Role
eksctl create iamserviceaccount --cluster=demo-cluster-1 --namespace=kube-system --name=aws-load-balancer-controller --role-name AmazonEKSLoadBalancerControllerRole --attach-policy-arn=arn:aws:iam::084375573395:policy/AWSLoadBalancerControllerIAMPolicy –approve

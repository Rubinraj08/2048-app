# 2048-app
*provided application load balancer to controll the number of requests the application
*To be easily accessible for end users using ingress and ingress controller
*Technologies using Aws and Kubernetes
*services used
  --IAM user
  --IAM poilicies
  --Elastic compute cloud
  --Elastic Kubernetes Service


#Deploy the deployment, service and Ingress
kubectl apply -f 2048_full.yaml

#Create IAM Policy
aws iam create-policy --policy-name AWSLoadBalancerControllerIAMPolicy --policy-document file://iam_policy.json

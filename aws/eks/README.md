# AWS-EKS Tutorial
## This is a AWS-EKS tutorial with CloudFormation and Fargate

What we are building
![Image1](assets/images/EKS-AWS-1.png)

![Image1](assets/images/EKS-AWS-2.png)

##### Create Cluster
eksctl create cluster --name=eksdemo1 \
                      --region=us-east-1 \
                      --zones=us-east-1a,us-east-1b \
                      --without-nodegroup

This will create the cluster without any nodegroup and nodes.

`kubectl get nodes` should not return any nodes  
`kubectl get clusters` should return the clusters list


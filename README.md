# Airflow K8S Terraform LDI


Created on 12/10/24 
Resources: https://github.com/xvanausloos/eks-airflow/blob/main/README.md

## Environments variables
Setup env variables 
`export AWS_PROFILE=sandbox`
`export AWS_DEFAULT_REGION=us-west-2`

## TF variables
Create `terraform/variables.tf`

## Provision VPC & cluster
Provision VPC & cluster : 
```
cd terraform
tf init
tf apply 
```

## Authenticate to AWS EKS cluster
```
aws eks update-kubeconfig --name sandbox-eks-cluster --region $AWS_DEFAULT_REGION 
```




# EKS Nginx Deployment

## Task Description
Create an AWS EKS cluster, deploy the Nginx application, and access the application from outside the cluster.

## Tech Stack
- AWS EKS (Kubernetes v1.33)
- eksctl
- kubectl
- AWS LoadBalancer

## Steps Performed

1. **Created EKS Cluster** using `eksctl` with a managed nodegroup (`eks-cluster-config.yaml`).
   - Region: `us-east-1`
   - Kubernetes version: `1.33`
   - Nodegroup: 2 x `t3.medium` managed workers

2. **Deployed Nginx** using `kubectl` (`nginx-deployment.yaml`, 2 replicas).

3. **Exposed the application externally** using a Kubernetes `LoadBalancer` service (`nginx-service.yaml`).

4. **Verified external access** via the AWS Elastic Load Balancer DNS in a browser.

## Application URL
http://a8b513f0a3f3a49f398d555a3ddf4cc1-726640172.us-east-1.elb.amazonaws.com

## Screenshots
See the `/screenshots` folder for step-by-step evidence.

## Project Files
- `eks-cluster-config.yaml` — EKS cluster + managed nodegroup definition
- `nginx-deployment.yaml` — Nginx deployment manifest
- `nginx-service.yaml` — LoadBalancer service manifest
- `README.md` — this file
- `screenshots/` — proof-of-work images
<<<<<<< HEAD
EOF
cat ~/eks-nginx-project/README.md
=======
>>>>>>> f22ba0a (Add YAML manifests)

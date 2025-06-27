# HTTPBin Deployment on AWS EKS

## Overview

This project deploys the kennethreitz/httpbin Docker image on an AWS EKS cluster. It exposes the `/get` endpoint publicly and the `/post` endpoint privately.

## Prerequisites

- AWS CLI
- Terraform
- kubectl

## Steps

1. **Set Up Terraform Configuration**: Define the VPC, subnets, and EKS cluster.
2. **Deploy Kubernetes Resources**: Create deployment, services, and ingress.
3. **Apply Terraform Configuration**: Initialize and apply Terraform.
4. **Deploy Kubernetes Resources**: Apply Kubernetes manifests.

## Endpoints

- Public: `http://public.example.com/get`
- Private: `http://private.example.com/post`

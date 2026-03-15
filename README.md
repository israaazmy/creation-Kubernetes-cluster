# creation-Kubernetes-cluster

# Kubernetes Cluster Setup

This repository documents the setup of a Kubernetes cluster using kubeadm.

## Cluster Architecture

- 1 Master Node (Control Plane)
- 1 Worker Node

## Environment

OS: Ubuntu 22.04  
Container Runtime: containerd  
Kubernetes Version: v1.29

## Components Installed

- kubeadm
- kubelet
- kubectl
- Flannel Network Plugin
- NGINX Ingress Controller

## Application

OWASP Juice Shop deployed using Kubernetes Deployment and exposed via NGINX Ingress.

## Repository Structure

cluster-setup/ : documentation for cluster creation  
manifests/ : Kubernetes deployment files  
monitoring/ : monitoring recommendations


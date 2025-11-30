# Kubernetes-DevOps-Labs

A growing collection of Kubernetes labs for DevOps & Cloud practice
(by Istiak / istiak-devsecops)

--- 

## Overview

This repo is a work in progress — I keep adding new Kubernetes examples as I learn, experiment, and build real DevOps workflows.
Think of it as a hands-on playground for Kubernetes: deployments, services, ingress, configs, autoscaling, Helm, and monitoring with Prometheus/Grafana.
If you’re learning Kubernetes or you want ready-to-run examples for your own cluster, you’ll find practical, minimal, and reusable manifests here.

---

## Current Labs

Here are the labs currently included (the list will grow over time):

…	more coming soon

(Expect regular updates as I add more labs.)

---

## How to Use
1. Clone the repo
```bash
git clone https://github.com/istiak-devsecops/kubernetes-devops-labs.git
cd kubernetes-devops-labs
```
2. Make sure you have the basics installed
```bash
kubectl
Docker
Minikube / Kind / k3d (any local cluster works)
Helm (for Helm labs)
```
3. Enter any lab folder and apply the manifests
```bash
cd deployments/
kubectl apply -f .
```
4. Clean up when finished
```bash
kubectl delete -f .
```
5. For Helm labs
```bash
cd helm/simple-chart
helm install demo .
```
6. For Monitoring labs
```bash
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm install monitor prometheus-community/kube-prometheus-stack
```
--- 

## Contribution

This is an open repo — contributions, suggestions, and improvements are welcome.
Keep it simple, clean, and practical — that’s the goal of these labs.

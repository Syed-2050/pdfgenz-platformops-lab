# Prometheus Monitoring

Prometheus was installed using Helm inside the Kubernetes monitoring namespace.

## Purpose

Prometheus collects Kubernetes and node-level metrics such as:

- CPU usage
- Memory usage
- Pod status
- Node health
- Network activity

## Commands Used

kubectl create namespace monitoring

helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

helm repo update

helm install prometheus prometheus-community/prometheus --namespace monitoring

kubectl get pods -n monitoring

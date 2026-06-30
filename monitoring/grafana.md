# Grafana Dashboard

Grafana was installed using the official Grafana Helm chart and connected to Prometheus as a data source.

## Purpose

Grafana visualizes metrics collected by Prometheus.

## Commands Used

helm repo add grafana https://grafana.github.io/helm-charts

helm repo update

helm install grafana grafana/grafana --namespace monitoring

kubectl get pods -n monitoring

kubectl port-forward -n monitoring service/grafana 3000:80

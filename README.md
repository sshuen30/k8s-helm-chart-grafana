# grafana-helm-chart
Deploy grafana on a Kubernetes Cluster using Helm Chart

- Create a Grafana namespace in your Kubernetes Cluster
```bash
kubectl create namespace grafana
```

- Deploy Grafana helm chart
```bash
helm install grafana grafana/grafana --namespace grafana
```

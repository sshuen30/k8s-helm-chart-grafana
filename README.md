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

- Retrieve the username and password
```bash
kubectl get secrets grafana -n grafana -o yaml
```

- Decode the password from base64
```bash
echo -n "cndfjtrls" | base64 --decode 
```


## GLPI Kubernetes Deployment (Local)

This README provides instructions to deploy and access a GLPI application with a MySQL database on a local Kubernetes cluster using a NodePort Service and kubectl port-forward.

### Apply the Manifest

Deploy the resources to your cluster:
```
kubectl apply -f glpi-k8s.yaml
```
### Verify Deployment

Check that the pods are running:
```
kubectl get pods
```

### Verify the GLPI Service:
```
kubectl get svc glpi
```

#### s GLPI Locally

Open your browser and navigate to http://localhost:30080 to access the GLPI web interface. Complete the GLPI setup wizard using the following MySQL credentials

#### Database Name: `glpi`

#### User: `glpi`

#### Password: `glpi`

### Host: `mysql`
`kubernetes: v1.25.3` `Minicube: v1.28.0`

## Run the project.
1. Apply base.
```bash
kubectl apply -k ./base

# Show all component.
kubectl get all

# Access applications deployed in minikube
minikube service the-service --url
```

2. Apply staging.
```bash
kubectl apply -k ./overlays/staging

# Show all component.
kubectl get all

# Access applications deployed in minikube
minikube service staging-the-service --url
```

3. Apply production.
```bash
kubectl apply -k ./overlays/production

# Show all component.
kubectl get all

# Access applications deployed in minikube
minikube service production-the-service --url
```

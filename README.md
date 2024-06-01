# hello world application for first steps on k8s

# Run the example

## provision

```bash
kubectl apply -f deployment.yaml
```

```bash
kubectl apply -f service.yaml
```

## deprovision

```bash
kubectl delete -f deployment.yaml
kubectl delete -f service.yaml
```

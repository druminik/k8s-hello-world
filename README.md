# hello world application for first steps on k8s

# Run the example using kubectl

## provision

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

## test

```bash
kubectl get deployment
kubectl get service
curl -vk http://localhost:80
```

## deprovision

```bash
kubectl delete -f deployment.yaml
kubectl delete -f service.yaml
```

# run the example using helm

## install helm

```bash
brew install helm
helm create hello-world
helm install hello-world ./hello-world
```

## test

```bash
curl -vk http://localhost:80
```

update the created deployment.yaml and service yaml with the values from the /templates directory.

apply the changes

```bash
helm upgrade hello-world ./hello-world
```

## test

```bash
curl -vk http://localhost:80
```

## deprovision

```bash
helm uninstall hello-world
```

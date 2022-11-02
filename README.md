# Execute
Verify the cluster
```bash
kubectl get pod
```

Later, create the config mongo and the secret

```bash
kubectl apply -f mongo-config.yaml
```
```bash
kubectl apply -f mongo-secret.yaml
```
now, create the deployment and service 
```bash
kubectl apply -f mongo.yaml
```

Finally, create the deployment and service of webapp
```bash
kubectl apply -f webapp.yaml
```

## TO CHECK RUNNING
```
minikube ip
```
get that ip and set the port that you use in the webapp service specifically in the NodePort to access to the content

# Several commands to use
get pods running
```
kubectl get pod
```

See logs of a pod
```
kubectl logs pod-name -f
```

Inspect a pod
```
kubectl describe pod pod-name
```
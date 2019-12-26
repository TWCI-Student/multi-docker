## Creating and Deleting objects

```bash
# Create an object by feeding a config file to Kubectl
$ kubectl apply -f <filename>
$ kubectl apply -f <dir_name>

# Delete an object
$ kubectl delete -f <filename>
$ kubectl delete <object_type> <object_name>
$ kubectl delete <dir_name>
```

## Satus of Objects

```bash
# Show Pods
$ kubectl get pods [-o wide]

# Show Services
$ kubectl get services

# Show Deployments
$ kubectl get deployments

# Show persistent volumes
$ kubectl get pv

# Show persistent volume claims
$ kubectl get pvc

# Get detailed info about an object
$ kubectl describe <object type> [<object name>]

# Get information about storage class
$ kubectl get storageclass
$ kubectl describe storageclass

# Update deployment
$ kubectl set image <object_type> / <object_name> <container_name>=<new image to use>
```

## Secrets

```bash
# Get secrets
$ kubectl get secrets

# Secrets have to be defined imperatively
kubectl create secret <secret_type> <secret_name> --from-literal key=value

# Secret types
- generic
- docker-registry
- tls # For HTTPS setup
```

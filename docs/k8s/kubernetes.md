## Creating and Deleting objects

```bash
# Create an object by feeding a config file to Kubectl
$ kubectl apply -f <filename>

# Delete an object
$ kubectl delete -f <filename>
```

## Satus of Objects

```bash
# Show Pods
$ kubectl get pods [-o wide]

# Show Services
$ kubectl get services

# Show Deployments
$ kubectl get deployments

# Get detailed info about an object
$ kubectl describe <object type> [<object name>]

# Update deployment
$ kubectl set image <object_type> / <object_name> <container_name>=<new image to use>
```

```bash
# Load config files
$ kubectl apply -f client-pod.yaml
pod/client-pod created

$ kubectl apply -f client-node-port.yaml
service/client-node-port created

# Get status of pods
$ kubectl get pods

# Get status of services
$ kubectl get services

# Show the container that is running via K8s
$ docker ps
```

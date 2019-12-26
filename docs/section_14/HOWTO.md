# Setup Project

```bash
# Run Kubernetes
$ kubectl create secret generic pgpassword --from-literal PGPASSWORD=12345asdfg
$ kubectl apply -f k8s

# Verify that server is running correctly
$ kubectl logs <server_deployment_id>
```

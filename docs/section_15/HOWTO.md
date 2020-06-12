## Ingress Setup

1. Download object configuration file:

   - Go to https://github.com/kubernetes/ingress-nginx or https://kubernetes.github.io/ingress-nginx/deploy/ or directly to https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/static/mandatory.yaml

2. Apply the configuration file to kubectl

   - Run the command: `kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/static/mandatory.yaml`

   - If you are using Docker Desktop's Kubernetes, then you have also to execut the following command:
     `kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/master/deploy/static/provider/cloud-generic.yaml`

3. Verify that the service is running:
   - `kubectl get svc -n ingress-nginx`

`

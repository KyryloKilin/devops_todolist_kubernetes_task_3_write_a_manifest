# How to apply manifests and test the Todo app

## 1. Create namespace and pods

```bash
# Apply namespace
kubectl apply -f _infrastructure/namespace.yml

# Apply busybox pod
kubectl apply -f _infrastructure/busybox.yml

# Apply todoapp pod
kubectl apply -f _infrastructure/todoapp-pod.yml

# Check that pods are running
kubectl get pods -n todoapp

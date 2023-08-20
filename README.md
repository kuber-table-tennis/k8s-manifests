# Kubernetes table-tennis
So the main purpose of this repo is to have the k8s manifests of the ping and pong services. The images are being pulled from a the docker repository of the sergiolv account. So, in order to this to work, we need to first pull the images out of there.

# Main commands
The below command is to create the namespace.
```
kubectl apply -f dev-namespace.yaml
```
The below command is to create the configmaps, deployments and services for each application.
```
kubectl apply -f ping-service.yaml
```
The bellow command is to enter a specific pod.
```
kubectl exec -it <POD-NAME> -n <NAMESPACE>
```
The bellow command is to see the logs of a pod.
```
kubectl logs <POD-NAME> -n <NAMESPACE>
```

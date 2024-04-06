# ENSF 400 - Assignment 3 - Kubernetes

## Steps
0. **Start Kubernetes**

minikube start
minikube addons enable ingress

1. **Create the Deployment for nginx:**

kubectl apply -f nginx-dep.yaml

2. **Create the ConfigMap for nginx:**

kubectl apply -f nginx-configmap.yaml

3. **Create the Service for nginx:**

kubectl apply -f nginx-svc.yaml

4. **Create the Ingress for nginx:**

kubectl apply -f nginx-ingress.yaml

5. **Create the Deployments and Services for app-1 and app-2:**

kubectl apply -f app-1-dep.yaml
kubectl apply -f app-1-svc.yaml
kubectl apply -f app-2-dep.yaml
kubectl apply -f app-2-svc.yaml

6. **Create the Ingresses for app-1 and app-2:**

kubectl apply -f app-1-ingress.yaml
kubectl apply -f app-2-ingress.yaml

7. **Test the setup:**

curl http://$(minikube ip)/
curl http://$(minikube ip)/


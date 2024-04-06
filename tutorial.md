# ENSF 400 - Assignment 3 - Kubernetes

## 

 **Compile**

minikube start && minikube addons enable ingress; kubectl apply -f nginx-dep.yaml; kubectl apply -f nginx-configmap.yaml; kubectl apply -f nginx-svc.yaml; kubectl apply -f nginx-ingress.yaml; kubectl apply -f app-1-dep.yaml; kubectl apply -f app-1-svc.yaml; kubectl apply -f app-2-dep.yaml; kubectl apply -f app-2-svc.yaml; kubectl apply -f app-1-ingress.yaml; kubectl apply -f app-2-ingress.yaml


NOTE: if it breaks, run the command(s) that failed one at a time, individually


**Test**

curl http://$(minikube ip)/; curl http://$(minikube ip)/; curl http://$(minikube ip)/; curl http://$(minikube ip)/

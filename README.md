# k8s

# 01 - Wordpress
````
git clone https://github.com/falconsoft3d/k8s.git
cd k8s
cd 01-wordpress
microk8s kubectl apply -f 00-namespace.yaml
microk8s kubectl get ns
microk8s kubectl -n testing apply -f 01-wordpress-service.yaml
microk8s kubectl -n testing get svc
microk8s kubectl -n testing apply -f 02-wordpress-rc.yaml
microk8s kubectl -n testing get pods
microk8s kubectl -n testing delete pod wordpress-j7cxt
microk8s kubectl get nodes -o wide
microk8s kubectl delete namespace testing
microk8s kubectl -n testing get ingress
````

````
microk8s kubectl get ingress
````
